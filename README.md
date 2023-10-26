# Sports-Competition-Corruption-Case-Study
Investigating three provided .pcap files using modern digital forensics techniques, looking for specified evidence of corruption and recovering it in a forensically sound manner.

## Introduction
This case study was produced by request of a national security agency to investigate an international sporting corruption case. Three network capture files were provided by the agency for the investigation, named “Capture 1.pcap, Capture 2.pcap, and Capture 3.pcap” respectively, each with a distinct set of data and aims defined by the client.

### Capture 1.pcap
The client requested an investigation into a potential case of bribery present within this packet capture; it was said to contain an undefined number of suspect details including names, aliases, and usernames, some of which may be obscured through the use of anti-forensic obfuscation techniques. The aim of the investigation into this packet is to recover said actor details and to describe the obfuscation techniques used and process of recovery.

### Capture 2.pcap
This file contains communications between a competition official and a foreign national agent and is described as containing File Transfer Protocol (FTP) traffic as well as other network packet types, indicating the exchange of confidential virtual files or folders. More forensic obfuscation techniques have been utilized in this exchange, with the client providing the clue that an Edward Snowden quote can aid in the deciphering process. The client asks for evidence of the files that were sent over, including a documented process of how this was deciphered and extracted.

### Capture 3.pcap
The third Capture file details communications between the actors Ill-Song and Ann Dercover, which the client suspects are attempting to schedule a discreet meeting. Details of the conversation (particularly the date and time of their meeting) are requested to be recovered for investigation purposes.

## Methodology
The use of a traditional forensic acquisition and analysis methodology such as OSCAR (Obtain Information, Strategize, Collect Evidence, Analyse, Report) would be ineffective throughout this investigation as the acquisition process has already been completed by the client and only the analysis and reporting stages need to be performed. In this instance, a more dynamic methodology focused on the analysis of network traffic needs to be utilized such as the Evidence Examination framework described in the US Department of Justice report: ‘Forensic Examination of Digital Evidence: A Guide for Law Enforcement’ (Ashcroft, et al., 2004). This was done following the steps mentioned in this guide – Preparation, Extraction, Analysis, Ownership and Possession, and finally Conclusion.

## Preparation
The preparation phase relates to getting the working directories ready to place extracted and recovered files into. The report recommends using separate media to store these files, however a simple desktop folder covered these requirements in this case. This is because the files do not need to be passed between investigators; this is an individual investigation with the results being passed on immediately to the client. 

## Extraction
As this is an entirely network packet-based investigation, typical operating system forensic methods mentioned in the standard methodology do not apply; the procedure instead focuses entirely on recovering requested data from the provided packet files. 
This includes the following:
-	Sent files and messages identified by Wireshark
-	Names and aliases
-	IP addresses
-	Suspicious port activity
-	Compressed data
-	Obfuscated data
-	Encrypted data
(The gathered data and working can be viewed in Appendix 1 of the Investigative Output file.)

## Analysis
Analysis is the act of recovering and understanding evidence from gathered data; it typically begins at the initial leads that triggers the investigation to be called such as noticeable network anomalies, compromised systems, or Intrusion Detection System alerts. Ashcroft et al’s Guide For Law Enforcement only covers the analysis of disk image contents, though in this case, the trigger was suspicious network packets. Data Analysis (and inherently, network packet analysis) requires the use of the following methods to develop a working conclusion, as noted by the European Union Agency for Cybersecurity (ENISA, 2016):
1.	Correlation – Gathering data from multiple sources to draw conclusions.
   
2.	Timeline – Creating a timeline from the gathered evidence.

### Ownership and Possession
To cover the requirements for establishing ‘Ownership and Possession,’ the following topics were investigated within the given files, building off the previous two steps of analysis.

3.	Events of Interest – Noting particular events that stand out or relate to the aims of the investigation.
   
4.	Corroboration – Verifying potential false positives using other sources.

### Conclusion
Finally, a conclusion was reached through the use of interpretation based on all the evidence gathered.

5.	Interpretation – Developing a working theory on the events that transpired.
