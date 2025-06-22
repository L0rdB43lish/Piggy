# Piggy

The piggy challange is not retired so I'm unable to share the writeup but I will give some context to what was the machine about, what I did and why.  

https://blueteamlabs.online/achievement/share/3356/66

---

In this lab, I was provided four packet capture (PCAP) files to analyse in order to identify unsual activities on the network.  

To locate SSH communications and find out which IP addresses were communicating with each other and transferring data, I applied "SSH" into the filter search bar. 

I used the `Statistics > Endpoints` feature to find out more information about data transferred between hosts.  

Several external IPs were found to be communicating with the infected system. I cross-referenced these IPs with `VirusTotal` where one address was flagged as malicious.  

Some IPs were communicating over non-standard ports. I noted the relevant ports and IPs using the `Destination and Ports` feature on Wireshark, then used `VirusTotal` to gather more information on them, including ASN data and threat intelligence.

In addition to the packet analisys, I performed basic OSINT tasks to complement the challange. 
