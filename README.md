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
Following searches for all the sites that is in the domain yahoo.com

![image](https://github.com/user-attachments/assets/61c7ccdb-a0cb-4efe-ac8d-36962cbb0b9e)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![image](https://github.com/user-attachments/assets/57a7da73-f8ca-4c58-a5c9-2516816d86af)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![Screenshot (349)](https://github.com/user-attachments/assets/9aded600-5ec2-4222-bf9f-c4e4cfcd03c2)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![image](https://github.com/user-attachments/assets/b7520cb7-840c-4f90-9094-0fa57983cb73)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![Screenshot (350)](https://github.com/user-attachments/assets/83adc5a3-480c-4827-b920-1abf6de03825)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/user-attachments/assets/20e69b44-d3dc-449c-a7c9-c02dbbba2e60)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![Screenshot 2025-03-15 140323](https://github.com/user-attachments/assets/5954971f-82e6-49f1-ac56-2ddad234c414)


 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![WhatsApp Image 2025-03-15 at 14 34 53_a828455d](https://github.com/user-attachments/assets/13b8974f-4c34-4e96-8ef4-ee14653d9840)







##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

![WhatsApp Image 2025-03-15 at 14 36 47_3cb3d733](https://github.com/user-attachments/assets/5f71b355-353b-41fe-ac54-87bb70117a84)

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


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![WhatsApp Image 2025-03-17 at 18 59 20_26c5d15d](https://github.com/user-attachments/assets/528acf94-f4f8-4b5b-af9d-be3f1f701cfc)




In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![WhatsApp Image 2025-03-17 at 18 50 22_5749286f](https://github.com/user-attachments/assets/063f9574-2da7-4d54-a5ec-cb7401121298)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
![WhatsApp Image 2025-03-15 at 14 41 47_de34368f](https://github.com/user-attachments/assets/07b0d504-0810-46c6-9336-e0602138d467)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![WhatsApp Image 2025-03-17 at 18 49 56_0dae7968](https://github.com/user-attachments/assets/3e9c911d-3d6f-4cfb-b2d8-592a8f4189f5)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

