### Talence Red Team Course

### Draft

### Chapter 1: Introduction to Red Teaming
1.1. Overview of Red Team Operations  
   1.1.1. Definition and Objectives of Red Teaming  
   1.1.2. Differences between Red Teaming and Penetration Testing  
1.2. Tools and Environment Setup  
   1.2.1. Overview of Tools  
   1.2.2. Setting Up a Red Teaming Lab Environment  

### Chapter 2: Reconnaissance and OSINT
2.1. Passive Reconnaissance  
   2.1.1. Techniques  
   2.1.2. Reconnaissance and OSINT Frameworks  
   Includes tools such as Maltego, Recon-ng, FOCA  
2.2. Active Reconnaissance  
   2.2.1. Network Scanning, Port Scanning, Service Enumeration  
   2.2.2. Active Reconnaissance Tools  
   Includes tools such as Nmap, Shodan, Masscan  
2.3. Social Engineering Recon  
   2.3.1. Gathering Information from Human Targets  
   2.3.2. Social Engineering Tools and Techniques  

### Chapter 3: Initial Access Techniques
3.1. Phishing Campaigns  
   3.1.1. Crafting Effective Phishing Emails  
   3.1.2. Phishing Frameworks  
   Includes tools such as Gophish  
3.2. Exploiting Public-Facing Applications  
   3.2.1. Web Application Exploitation Techniques  
   Topics include SQLi, RCE, XSS  
   3.2.2. Case Study: Real-World Exploits  
   Example: ProxyShell  
3.3. Social Engineering  
   3.3.1. Advanced Social Engineering Techniques  
   3.3.2. Social Engineering Tools and Techniques  
3.4. Malicious Documents for Initial Access  
   3.4.1. Staged / Stageless Payload  
   3.4.2. Stealth Payload Generation  
   3.4.3. Macros in Office Files  
   3.4.4. Infected PDF and Known Exploits  
   3.4.5. PowerShell Downgrade Attacks  
   3.4.6. LNK File (Shortcuts) Attacks  
3.5. Advanced Techniques  
   3.5.1. Domain Fronting  
   3.5.2. Tunneling Techniques  

### Chapter 4: Code Exection
4.1. Bypassing Application Whitelisting  
4.2  In-Memory PowerShell   
4.3. Living off the Land Binaries (LOLBins)  
   4.3.1. Practical Examples: Rundll32.exe, Regsvr32.exe, MSHTA.exe, Certutil.exe  
   4.3.2. LOLBins Downsides and Limitations due to Detection and Monitoring  
4.4. XSL Script Processing  
4.5. Inline C# Code Execution  
4.6. Process Injection and Hijacking  
   4.6.1. DLL Injection  
   4.6.2. Reflective DLL Injection  
   4.6.3. Remote Thread Injection  
   4.6.4. APC Injection  
   4.6.5. Thread Hijacking  
   4.6.6. PE Injection  
   4.6.7. IAT Hooking and Inline Hooking  
   4.6.8. Process Hollowing  
   4.6.9. Direct Syscalls  
   
### Chapter 5: Persistence Techniques
5.1. Persistence via Scheduled Tasks  
   5.1.1. Creating and Managing Scheduled Tasks  
   5.1.2. Task Obfuscation Techniques  
5.2. Registry Persistence  
   5.2.1. Popular Windows Registry Keys for Persistence  
   5.2.2. Avoiding Detection through Obscured Registry Changes  
5.3. WMI and Service Persistence  
   5.3.1. WMI Event Subscription for Persistence  
   5.3.2. Service and DLL Hijacking  
5.4. Persistence via Valid Accounts  
5.5. Advanced Persistence Techniques  
   5.5.1. Rootkits and Bootkits  
   5.5.2. Hidden and Staggered Payloads for Delayed Execution  

### Chapter 6: Privilege Escalation
6.1. Local Privilege Escalation on Windows  
   6.1.1. UAC Bypass Techniques  
   6.1.2. Token Impersonation  
   6.1.3. Exploiting Vulnerable Services (e.g., PrintNightmare)  
6.2. Linux Privilege Escalation  
   6.2.1. Sudo Misconfigurations  
   6.2.2. Cron Job Exploitation  
   6.2.3. Kernel Exploits (e.g., Dirty COW)  
6.3. Exploiting Misconfigurations  
   6.3.1. File and Directory Permissions  
   6.3.2. Service Misconfigurations  

### Chapter 7: Defense Evasion
7.1. Obfuscation Techniques  
   7.1.1. Script and Binary Obfuscation  
   7.2.1. PowerShell Obfuscation  
7.2. Disabling and Deleting Logs  
   7.2.1. Avoid ETW Logging  
   7.2.2. Modifying or Deleting Logs  
7.3. Security Tools Evasion  
   7.3.1. EDR/AV Solutions Attack Surface
   7.3.2. BYOVD (Bring Your Own Vulnerable Driver) Techniques  
   7.3.3. AMSI Bypass Techniques  
7.4. Other Evasion Techniques  
   7.4.1. Fileless Malware Techniques  
   7.4.2. Living off the Land Binaries (LOLBins)  
   7.4.3. Using Fake Certificates to Sign Executables  

### Chapter 8: Credential Access
8.1. Credential Dumping  
   8.1.1. Windows Credential Dumping  
   Includes tools such as Mimikatz, Rubeus, SharpHound  
   8.1.2. Techniques: NTLM Hash Extraction, Pass-the-Hash  
   8.1.3. Linux Credential Dumping  
   Techniques: Extracting Passwords from Memory  
   8.1.4. Overview of LSASS Dump Techniques  
   Techniques: Direct Dumping of LSASS Memory, Remote LSASS Dumping via PsExec, Lsassy (Rundll32.exe/comsvcs.dll)  
8.2. Pass-the-Hash and Pass-the-Ticket  
   8.2.1. NTLM Relay Attacks  
   8.2.2. Kerberos Ticket Attacks (Silver Ticket, Golden Ticket)  
8.3. Other Credential Access Techniques  
   8.3.1. Credential Harvesting from Web Browsers  
   8.3.2. Keylogging Techniques  

### Chapter 9: Pivoting and Lateral Movement
9.1. RDP, SMB, and WMI Exploitation  
   9.1.1. Using RDP for Lateral Movement  
   9.1.2. PsExec for Remote Command Execution  
   9.1.3. Leveraging SMB and WMI for Lateral Movement  
9.2. Tunneling Techniques to Move from a Subnet to Another  
   9.2.1. Tunneling  
   9.2.2. Socks Proxy  
9.3. Lateral Movement Tools and Techniques  
   9.3.1. PowerShell Remoting and WinRM  
   9.3.2. Custom Scripting for Lateral Movement  

### Chapter 10: Domain Escalation
10.1. AD Enumeration and Exploitation  
   10.1.1. ACLs in Active Directory  
   10.1.2. Locating and Enumerating Domain Admin Accounts  
   10.1.3. Mapping AD with BloodHound  
10.2. Exploiting Trust Relationships  
   10.2.1. Attack Paths via Trust Relationships  
10.3. Domain Controller Attacks  
   10.3.1. Kerberoasting, DCSync, DCShadow, and Other DC Exploits  
10.4. Gaining and Maintaining Domain Admin Access  
   10.4.1. Techniques for Persistence within the Domain  
10.5. Cross-Forest and Cross-Domain Escalation  
   10.5.1. Attacking Multiple Domains and Forests  

### Chapter 11: Command and Control (C2)
11.1. Setting Up C2 Infrastructure  
   11.1.1. Overview of C2 Tools  
   Examples: Cobalt Strike, Empire, Covenant  
   11.1.2. Building a Resilient C2 Infrastructure  
   Techniques: Domain Fronting, Redirectors  
11.2. Payload Development and AV Evasion  
   11.2.1. Obfuscation, Shellcode, Encoders  
   11.2.2. Bypassing EDR and AV with Custom Payloads  
11.3. C2 Communication Channels  
   11.3.1. HTTP/S, DNS, and Custom Protocols  
   11.3.2. Steganography and Covert Channels for C2  
11.4. Advanced C2 Techniques  
   11.4.1. Steganography, Domain Fronting, Covert Channels  
   11.4.2. Managing C2 in Complex Environments  
11.5. Case Study: Real-World C2 Operations  
   11.5.1. Analysis of High-Profile C2 Scenarios  

### Chapter 12: Data Exfiltration
12.1. Data Exfiltration Over Common Protocols  
   12.1.1. HTTP, HTTPS, and DNS Tunneling Techniques  
   12.1.2. Leveraging Cloud Services for Exfiltration  
12.2. Covert Data Exfiltration  
   12.2.1. Exfiltrating Data Over Non-Traditional Channels  
   12.2.2. Encryption and Steganography for Data Exfiltration  

### Chapter 13: Post-Exploitation and Reporting
13.1. Maintaining Access  
   13.1.1. Techniques for Long-Term Persistence  
   13.1.2. Cleanup and Avoiding Detection  
13.2. Evidence Gathering and Reporting  
   13.2.1. Collecting Evidence and Artifacts  
   13.2.2. Crafting a Comprehensive Red Team Report  
13.3. Lessons Learned and Remediation Recommendations  
   13.3.1. Analyzing Gaps and Strengthening Defenses  
   13.3.2. Collaborating with Blue Teams
   13.3.2. Continuous Improvement 

### Conclusions
