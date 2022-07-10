# Tools of the trade

Name | Description
-- | - 
`exiftool` | read EXIF data from images for digital forensics
`gobuster` | brute force directories and pages
`nslookup` | look up DNS records
`pdfinfo` | view PDF metadata for digital forensics

### ExifTool

```bash
sudo apt install libimage-exiftool-perl

exiftool IMAGE.png
```

### Gobuster

```bash
sudo apt-get -y install gobuster

gobuster -u http://website.com -w wordlist.txt dir
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