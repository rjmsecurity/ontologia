# Phishing

* social engineering and a bit of spoofing
* often delivered by email, text, etc.
* always check the URL; better yet, don't click links in emails, instead type the URL of the website you want to go to in the browser
	* **typosquatting ⟹** a type of URL hijacking
		* *professormessor.com*
		* **prepending ⟹** *pprofessormesser.com*
* also check for typos or something wrong with the graphics or font, e.g. something looks off about the login form
* you can also check if links on the spoofed website work, e.g. are the footer links all not working?

* **pretexting ⟹** when an attacker lies to a victim to get information from them, creating a situation and trying to get the victim to act on it
	* *hello, we are calling from Visa regarding an automated payment to your utility service...*
	* the victim may feel relaxed by this statement coming from the attacker if the victim does, in fact, have automated payments set up for their utility service
	* the 2015 TalkTalk data breach is a good example of pretexting, where attackers called customers and gave them details about their accounts, their address, etc. as part of a vishing attack
		* of course, the attackers stole this information and were using it to extract more sensitive information, such as credit cards, directly from the customers
		* nevertheless, customers felt relaxed enough to give out sensitive information and did not know that TalkTalk does not resolve payment issues by calling customers and giving them their account details and asking for their credit card number

* **pharming ⟹** instead of targeting individuals, now we are targeting groups of people
	* legitimate website redirects to bogus site via poisoned DNS server or by the legitimate website directly being hacked
	* in this case, checking the URL in the browser does not help victims
* remember, **pharming** is redirecting large groups of people, **phishing** is the collection of credentials, so attackers combine pharming with phishing
* both people and antivirus/anti-malware have a hard time detecting pharming because everything appears normal; thankfully pharming is a rare attack but you need to know how to mitigate it on your network #todo learn how

* **vishing ⟹** performing phishing over a voice line; often the phone number is spoofed; again, the goal is for the attacker to gain personal information to be able to access your accounts

* **smishing (SMS phishing) ⟹** phishing done over text message communication; spoofing also occurs here; often includes a link to click

* extra credit: stay up to date on the many variations of scams out there that try to entice you into giving up information or money, go to https://reddit.com/r/scams
	* fake check scam, phone verification code scam, Boss/CEO scam, advance-fee scam

* **spear phishing ⟹** phishing targeted at specific person or group of people
	* **whaling ⟹** spear phishing where the victim is a high-profile individual with a lot of money or information, usually a CEO or CFO/head of accounting because they have access to the entire corporate bank account
	* reconnaissance: attacker needs to gather as much intel on the victim as possible
		* so much information on any individual, group, or organization is open source; all the attacker needs to do is visit lead generation sites, LinkedIn, Twitter, Facebook, Instagram, the corporate website, etc.
		* with enough information, the attacker can build a very believable pretext, gathering where you live, where you bank, where you work, who you work with, use people's name, understand places you shop, etc.
		* for this reason, CEOs and CFOs and others in charge of corporate accounts must be aware of phishing attacks and how easy it is to be convinced to log in to a fake user account and give out banking information

#securityplus **1.1** *Compare and contrast different types of social engineering techniques.*