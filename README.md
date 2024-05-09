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

![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/9e155b91-c2b5-461e-9fbf-96bf29be0b84)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/1c35d800-b632-4b46-b009-17af408ef5be)




intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/23ecdd50-cad4-4600-ad72-a288a6890336)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/d8924e4e-170b-4629-b8ae-ed3c0ff1f4e9)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/43dd1c32-b5cd-4306-9c9e-0359375e0bc3)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/8edca968-69d6-4fff-b240-4dcbf19b638e)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/d99827cd-a1dd-430e-a1ed-80998fd7d65a)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/3ce4766b-8d50-4c73-a53b-d8c573f381c0)







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
![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/35d3e8b7-2df9-4533-b7a5-330eca7d5f64)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/d4c7fcd1-d1c6-48ec-8a3d-5988a2bfe3f9)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/f15fbacf-86f7-48cb-a4ac-4615b4ba02fc)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
 ![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/b1c33033-d132-41f1-aba3-4b2aa796048a)

  
  

## nmap –script smtp-enum-users.nse <hostname>
![image](https://github.com/srinivasanvaiyali/Enumeration/assets/145117665/565029b9-d087-47df-bb0e-fe9c42e46d13)

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

