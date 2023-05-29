# Enumeration

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

### Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

#### site: 
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain youtube.com

![githubsite](https://github.com/Guru-Guna/Enumeration/assets/93427255/d780bc33-3f2b-45ef-b817-f9b5a1cc143a)





##### filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain youtube.com

![filetype](https://github.com/Guru-Guna/Enumeration/assets/93427255/85aa8850-8284-4dc1-b71f-8f6a54a25d89)




#### intext: 
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![passcode](https://github.com/Guru-Guna/Enumeration/assets/93427255/ffb53de9-b9ec-4c5f-a4ba-de3da324ea2c)




#### inurl: 
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![inurl](https://github.com/Guru-Guna/Enumeration/assets/93427255/e9a609a2-dd1d-4459-b15b-e9008d3bdb58)




#### intitle: 
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![inurl index](https://github.com/Guru-Guna/Enumeration/assets/93427255/bfcd36d6-42c3-4f57-8d0e-d0e42876d508)







#### link:
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![example](https://github.com/Guru-Guna/Enumeration/assets/93427255/5f6a8c01-49f8-4289-9073-92a2f08d02b0)





#### cache: 
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![cacheexample](https://github.com/Guru-Guna/Enumeration/assets/93427255/1f87ebdf-87fa-4182-b5d7-c015ee6fdc18)


# DNS Enumeration

## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![brew](https://github.com/Guru-Guna/Enumeration/assets/93427255/db096c40-c03a-414d-8a16-e5b02e4715b6)


![cdac](https://github.com/Guru-Guna/Enumeration/assets/93427255/d4cee9ee-9b23-4bc2-8637-140030554217)




## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.


![enum](https://github.com/Guru-Guna/Enumeration/assets/93427255/c514a318-8911-4303-a6c7-5399c8a9a585)




## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![usrenum](https://github.com/Guru-Guna/Enumeration/assets/93427255/a4a69105-b904-4220-95df-d1232c362c4d)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![smpt](https://github.com/Guru-Guna/Enumeration/assets/93427255/f6ec2244-8704-485f-9af2-e0db28afec93)



select any username in the first column of the above file and check the same

![proxy](https://github.com/Guru-Guna/Enumeration/assets/93427255/8314eedc-bcc2-49cf-a539-bd58256e35aa)



# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
## Output:
  
![telnet](https://github.com/Guru-Guna/Enumeration/assets/93427255/69004450-8501-41b9-a66d-dd7c1ddf2101)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![telnet out](https://github.com/Guru-Guna/Enumeration/assets/93427255/144f8877-d80e-4df4-ba31-4428bab1383d)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

