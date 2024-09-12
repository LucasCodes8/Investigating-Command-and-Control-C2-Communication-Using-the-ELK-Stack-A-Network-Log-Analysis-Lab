# Investigating Command and Control (C2) Communication Using the ELK Stack

## Overview

This lab involves analyzing network connection logs to identify potential Command and Control (C2) communication using the ELK Stack. The investigation is based on the "ItsyBitsy" challenge from TryHackMe, simulating a real-world scenario where a suspected user, Browne, is potentially involved in malicious activity.

## Objectives

- Analyze HTTP connection logs using Kibana to identify suspicious C2 communication.
- Investigate IP addresses and patterns to uncover malicious activity.
- Understand how legitimate tools can be abused for malicious purposes.

## Lab Environment

- Platform: TryHackMe - ItsyBitsy Challenge
- Tools: ELK Stack (Elasticsearch, Logstash, Kibana), AbuseIPDB

## Step-by-Step Process

1. **Establishing the Timeline**:  
   Set the date range to March 2022 and identify periods of significant activity.

2. **Identifying the Suspect's IP Address**:  
   Analyze log activity percentages to identify the IP address associated with the suspect user.

3. **Analyzing the Malicious Activity**:  
   Determine the legitimate Windows binary used for the download from the C2 server.

4. **Identifying the Accessed File**:  
   Locate the file accessed during the breach and retrieve the flag from the associated Pastebin link.

## Tools and Technologies Used

- **ELK Stack (Elasticsearch, Logstash, Kibana)**
- **AbuseIPDB**
- **TryHackMe Platform**
- **Command Line Tools (bitsadmin)**

## Results and Analysis

- Identified C2 communication involving the use of `bitsadmin` to download files from Pastebin.
- Discovered the IP address and URL involved in the malicious activity.

## Challenges Faced

- Limited data availability and initial misinterpretation of log data.
- Dependency on external databases for IP reputation checks.

## Conclusion

The lab demonstrated effective use of the ELK Stack to identify and investigate C2 communications, emphasizing the importance of analyzing various network traffic patterns.

## Full Write-Up

For the complete write-up, please see the [full report here](https://github.com/LucasCodes8/Investigating-Command-and-Control-C2-Communication-Using-the-ELK-Stack-A-Network-Log-Analysis-Lab/blob/main/Investigating%20Command%20and%20Control%20(C2)%20Communication%20Using%20the%20ELK%20Stack_%20A%20Network%20Log%20Analysis%20Lab.pdf).

## References

- [Elastic Stack Documentation](https://www.elastic.co/guide/index.html)
- [AbuseIPDB](https://www.abuseipdb.com)
- [TryHackMe - ItsyBitsy Challenge](https://www.tryhackme.com)
