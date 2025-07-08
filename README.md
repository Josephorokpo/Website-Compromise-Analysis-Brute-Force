# **Website Compromise Analysis \- Brute Force Attack**

## **Project Introduction**

This project documents the investigation of a cybersecurity incident affecting yummyrecipesforme.com, where visitors were redirected to a malicious website after downloading an executable file. As a cybersecurity analyst, I analyzed network traffic to understand the attack chain, identified the initial compromise vector (brute force), and documented the incident. This exercise demonstrates skills in incident investigation, network protocol analysis, and recommending security measures.

## **Methodology and Analysis**

The investigation began after multiple customer complaints about unusual website behavior and slow computers. The issue was replicated in a sandbox environment, observing the download prompt and subsequent redirection. Network traffic was captured using tcpdump to analyze the communication flow.

My methodology involved:

1. **Incident Replication & Observation:** Confirming the reported symptoms and behavior in a controlled sandbox.  
2. **Network Traffic Analysis:** Examining the tcpdump log to trace the communication path, identify involved protocols (DNS, HTTP), and pinpoint the redirection mechanism.  
3. **Protocol Identification:** Determining how DNS and HTTP were utilized in the initial website access and the subsequent malicious redirection.  
4. **Compromise Vector Confirmation:** Correlating network observations with information about the brute force attack on the web host's administrative account.  
5. **Incident Documentation:** Detailing the sequence of events, symptoms, and discovered information.  
6. **Remediation Recommendation:** Proposing a specific security measure to prevent future brute force attacks.

## **Incident Report & Findings**

A comprehensive incident report, detailing the network protocol analysis, incident documentation, and a recommendation for brute force prevention, is provided in the Website\_Compromise\_Incident\_Report.md file within this repository.

## **Key Learnings**

This activity reinforced the importance of:

* Understanding how common network protocols (DNS, HTTP) are used in both legitimate and malicious contexts.  
* The critical role of strong authentication and brute force prevention in securing web applications.  
* Analyzing network traffic to trace attack paths and identify indicators of compromise.  
* The importance of detailed incident documentation for effective response and future prevention.  
* Recognizing the dangers of client-side redirection via injected code.