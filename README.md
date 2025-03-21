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

# Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain myntra.com

![Screenshot (44)](https://github.com/user-attachments/assets/fd090d94-467a-494f-885a-d1a1c7455639)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![Screenshot (45)](https://github.com/user-attachments/assets/09aa3211-3631-42e3-ae47-9653f0feb723)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![Screenshot (46)](https://github.com/user-attachments/assets/d3825407-49e7-4c6d-8570-e63fc1ad2faa)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![Screenshot (47)](https://github.com/user-attachments/assets/61a67643-7fa1-4e9b-b7f5-de8c1f02892b)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![Screenshot (48)](https://github.com/user-attachments/assets/5e2c12cd-9335-4a9d-9f4f-72d4eec198e7)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![Screenshot (49)](https://github.com/user-attachments/assets/f55fa3f7-97be-478c-b849-5c62ed71ca21)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:



![Screenshot (50)](https://github.com/user-attachments/assets/1854bc31-f10f-4a24-b2f6-a9c4daedf8f1)




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

## OUTPUT

![Screenshot (51)](https://github.com/user-attachments/assets/54ff3665-2f5d-4f7d-aee4-b722c5a2ccab)

![Screenshot (52)](https://github.com/user-attachments/assets/0a757656-3f56-48db-bd2e-16f99fcd43e0)


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
## OUTPUT 

![Screenshot (53)](https://github.com/user-attachments/assets/46df795e-5c69-4d20-9bc5-a2686e08c728)

## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
 ## Output
  
 ![Capture1](https://github.com/user-attachments/assets/8ee7a0b8-eefa-48d4-8879-70c947bfe5e6)
 

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![Capture 2](https://github.com/user-attachments/assets/fb2b5ca4-7fb2-4c51-ba7f-1e8928e13546)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

