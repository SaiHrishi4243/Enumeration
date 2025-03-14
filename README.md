# Enumeration
Enumeration Techniques

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

## Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

## site: 
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

![WhatsApp Image 2025-03-10 at 11 35 31_66067782](https://github.com/user-attachments/assets/2728cfbe-c2a8-4c2a-8c2b-966fcdf72a4a)


## filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain youtube.com

![WhatsApp Image 2025-03-10 at 11 35 31_aca2838a](https://github.com/user-attachments/assets/ade2d22d-e221-46f5-af5b-55eaffbc995a)


## intext: 
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![WhatsApp Image 2025-03-10 at 11 35 31_64e70d72](https://github.com/user-attachments/assets/9a7dac25-7c45-4bb3-9d34-537c2723308f)


## inurl: 
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![WhatsApp Image 2025-03-10 at 11 35 32_9aca4ef7](https://github.com/user-attachments/assets/f9585be1-6aa0-45d0-8919-e9f04d8ea788)


## intitle: 
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![WhatsApp Image 2025-03-10 at 11 35 31_7efa942c](https://github.com/user-attachments/assets/c488de79-faff-4193-b2ab-c04e4fb4a5ff)


## link: 
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![WhatsApp Image 2025-03-10 at 11 35 31_33459338](https://github.com/user-attachments/assets/977a4558-4646-45ef-bb93-bcff1ea7901c)


## cache: 
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![Screenshot 2025-03-11 143455](https://github.com/user-attachments/assets/a746d574-7fa8-4a58-9f49-1c7e5223c7d0)

## DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![Screenshot 2025-03-10 113347](https://github.com/user-attachments/assets/f57ef2a0-63f7-4428-b78d-f9bf9344294f)

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

![Screenshot 2025-03-10 113402](https://github.com/user-attachments/assets/2100f70c-f914-4b09-b3f7-49163746606c)
![Screenshot 2025-03-10 113422](https://github.com/user-attachments/assets/e1ce01a1-8ef2-49f2-80ee-d1ac83826db4)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![Screenshot 2025-03-10 113549](https://github.com/user-attachments/assets/a8865b34-de0d-4c47-beb9-f9d3d69e0fdd)


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  
![Screenshot 2025-03-11 144104](https://github.com/user-attachments/assets/dabc5c03-93a5-4268-8487-b5e26d1b4835)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
![Screenshot 2025-03-10 113610](https://github.com/user-attachments/assets/4b95618d-ce79-4836-8665-4c16863926a3)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully.
