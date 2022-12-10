# Tools of the trade

Name | Description
-- | - 
`curl` | GET or POST
`dirb` | brute force directories and filenames
`dnsrecon` | enumerate subdomains
`exiftool` | read EXIF data from images for digital forensics
[`ffuf`](https://github.com/ffuf/ffuf) | brute force directories and filenames, even subdomains
`gobuster` | brute force directories and filenames
`hexeditor` | edit file as hex
`md5sum` | get md5 hash of something like a favicon
`nslookup` | look up DNS records
`pdfinfo` | view PDF metadata for digital forensics
[`sublist3r`](https://github.com/aboul3la/Sublist3r) | enumerate subdomains with OSINT

### curl
```bash
curl 'http://10.10.98.149/customers/reset?email=robert@acmeitsupport.thm' -H 'Content-Type: application/x-www-form-urlencoded' -d 'username=robert&email={username}@customer.acmeitsupport.thm'
```

### dirb
```bash
dirb http://10.10.244.37/ /usr/share/wordlists/SecLists/Discovery/Web-Content/common.txt
```

### dnsrecon

```bash
dnsrecon -t brt -d acmeitsupport.thm
```

### ExifTool

```bash
sudo apt install libimage-exiftool-perl

exiftool IMAGE.png
```

### ffuf

```bash
ffuf -w /usr/share/wordlists/SecLists/Discovery/Web-Content/common.txt -u http://10.10.244.37/FUZZ

# enumerate subdomains by looking at server responses
ffuf -w /usr/share/wordlists/SecLists/Discovery/DNS/namelist.txt -H "Host: FUZZ.acmeitsupport.thm" -u http://10.10.54.8
ffuf -w /usr/share/wordlists/SecLists/Discovery/DNS/namelist.txt -H "Host: FUZZ.acmeitsupport.thm" -u http://10.10.54.8 -fs {SIZE} # where {SIZE} is most commonly occuring "size" from previous command

# to enumerate usernames using an example website, POST request, and error response
ffuf -w /usr/share/wordlists/SecLists/Usernames/Names/names.txt -X POST -d "username=FUZZ&email=x&password=x&cpassword=x" -H "Content-Type: application/x-www-form-urlencoded" -u http://10.10.98.149/customers/signup -mr "username already exists"

# to crack a username and password combination
ffuf -w valid_usernames.txt:W1,/usr/share/wordlists/SecLists/Passwords/Common-Credentials/10-million-password-list-top-100.txt:W2 -X POST -d "username=W1&password=W2" -H "Content-Type: application/x-www-form-urlencoded" -u http://10.10.98.149/customers/login -fc 200 # where 200 ok is incorrect password, 302 found is correct password
```

### Gobuster

```bash
sudo apt-get -y install gobuster

gobuster -u http://website.com -w wordlist.txt dir

gobuster dir --url http://10.10.244.37/ -w /usr/share/wordlists/SecLists/Discovery/Web-Content/common.txt
```

### md5sum

```bash
curl https://static-labs.tryhackme.cloud/sites/favicon/images/favicon.ico | md5sum
# and then search https://wiki.owasp.org/index.php/OWASP_favicon_database 
```

### Nslookup

```bash
nslookup website.thm

nslookup --type=CNAME shop.website.thm
```

### Pdfinfo

```bash
sudo apt install poppler-utils

pdfinfo DOCUMENT.pdf
```

### sublist3r

```bash
./sublist3r.py -d acmeitsupport.thm
```