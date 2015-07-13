# N0D
Null0 Defense - project to design a tool for small companies who don't use firewalls or proxies to filter malicious traffic

Contributors included in alphabetical order  
@c0mmand3r420  
@Impatient4truth  
@lojikil  
@grc_ninja  
@_sw17ch  

#(Null0 Defense)

##Project Summary  
The purpose of this project is to build a tool for organizations that do not have firewalls or web proxies to filter malicious traffic
##Development Plan
###1. Phase 1 - BareBones - Severely Manual
####1.1 Read a Text File list of domains from a directory
####1.2 Find the current IP address of the domain
####1.3 Ping the domain on port 80 and register if it is UP or Down
1.3.1 Write the results to a text file `"SOC-Null0_Malware_Status_YYYYMMDD.txt`  
**_Domain Name_**  
**_IP address_**  
**_UP/DOWN status_**  
If it is UP:  Write the results to a text file `SOC-Null0_Malware_RuleAdditions_YYYYMMDD.txt [Null0 config statement]`  
If it is DOWN: Write the results to a text file `SOC-Null0_Malware_RuleRemoval_YYYYMMDD.txt [Null0 config statement]`  	
####1.4 Maintain a Master list of what's being Null routed (adding and removing as needed)
###2.  Phase 2 - Add Meat - Partial Automation
####2.1 Email the text files to a person or group
###3.  Phase 3 - Add Skin - Mostly Automated
####3.1 Use an API to pull the malware domain name changes (adds/deleted) from malwaredomains.com
###4. Phase 4 - Add Brain - Fully Automated
####4.1 One button click for network team to update the router
###5. Phase 5 &amp; Forward - Shopping for Accessories - Enhancements
####5.1 Add different intel sources to pull malware domain lists from
