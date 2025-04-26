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

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain linkedin.com

![Screenshot (15)](https://github.com/user-attachments/assets/2d168b76-2dba-4138-b592-1ca886a1be91)



filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain linkedin.com


![Screenshot (16)](https://github.com/user-attachments/assets/84f130c6-f5f1-4206-a0b3-8c51619c8f59)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.


![Screenshot (17)](https://github.com/user-attachments/assets/86baa351-d834-4ad6-a6cb-3f5b0d69bbb0)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:Hafeezul" would search for pages that contain the word "admin" within the URL.

![Screenshot (18)](https://github.com/user-attachments/assets/f35f2d30-ea9d-498c-b5a5-cfe919bb7ff0)



intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:Networkchuck of" would search for pages that contain "index of" within the title tag.

![Screenshot (19)](https://github.com/user-attachments/assets/6564cc3d-e90d-4f97-adf7-be2064672832)





link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.


![Screenshot (20)](https://github.com/user-attachments/assets/95413c1c-451a-4dc7-8228-6fa390ea6ebc)



cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.



![Screenshot (21)](https://github.com/user-attachments/assets/8b5a8a76-8146-4c3c-b437-ea32952ca44e)


 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![dnsrecon](https://github.com/user-attachments/assets/311b8cbd-ed99-4a59-b00f-38dfbfc3c60b)




##dnsenum
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
##OUTPUT:

![dnsenum](https://github.com/user-attachments/assets/6ce5d9a4-2f06-497b-b1e4-b8ff69d81ee0)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
##OUTPUT:

![enm](https://github.com/user-attachments/assets/3e426389-8cbe-4ae6-8335-25b040856d8d)



In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:



select any username in the first column of the above file and check the same




#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands  
 
 ##Output
 
![telnet og](https://github.com/user-attachments/assets/6d90fda2-8e05-41e0-8762-7ad07b987b44)


  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:

![nmap script](https://github.com/user-attachments/assets/7d265d72-e928-4e90-915d-3c9ac5246847)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

