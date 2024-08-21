### Talence Red Team Course

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
   - Tools: Maltego, Recon-ng, FOCA  
2.2. Active Reconnaissance  
   2.2.1. Network Scanning, Port Scanning, Service Enumeration  
   2.2.2. Active Reconnaissance Tools  
   - Tools: Nmap, Shodan, Masscan  
2.3. Social Engineering Recon  
   2.3.1. Gathering Information from Human Targets  
   2.3.2. Social Engineering Tools and Techniques  

### Chapter 3: Initial Access Techniques
3.1. Phishing Campaigns  
   3.1.1. Crafting Effective Phishing Emails  
   3.1.2. Phishing Frameworks  
   - Tools: Gophish  
3.2. Exploiting Public-Facing Applications  
   3.2.1. Web Application Exploitation Techniques  
   - Topics: SQLi, RCE, XSS  
   3.2.2. Case Study: Real-World Exploits  
   - Example: ProxyShell  
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

### Chapter 4: Initial Access Techniques -> NEW !!!
4.1. Bypassing Application Whitelisting  
4.2. Living off the Land Binaries (LOLBins)  
   4.2.1. Practical Examples: Rundll32.exe, Regsvr32.exe, MSHTA.exe, Certutil.exe  
   4.2.2. LOLBins Downsides and Limitations due to Detection and Monitoring  
4.3. XSL Script Processing  

### Chapter 4: Persistence Techniques
4.1. Persistence via Scheduled Tasks  
   4.1.1. Creating and Managing Scheduled Tasks  
   4.1.2. Task Obfuscation Techniques  
4.2. Registry Persistence  
   4.2.1. Popular Windows Registry Keys for Persistence  
   4.2.2. Avoiding Detection through Obscured Registry Changes  
4.3. WMI and Service Persistence  
   4.3.1. WMI Event Subscription for Persistence  
   4.3.2. Service and DLL Hijacking  
4.4. Persistence via Valid Accounts  
4.5. Advanced Persistence Techniques  
   4.5.1. Rootkits and Bootkits  
   4.5.2. Hidden and Staggered Payloads for Delayed Execution  

### Chapter 5: Privilege Escalation
5.1. Local Privilege Escalation on Windows  
   5.1.1. UAC Bypass Techniques  
   5.1.2. Token Impersonation  
   5.1.3. Exploiting Vulnerable Services (e.g., PrintNightmare)  
5.2. Linux Privilege Escalation  
   5.2.1. Sudo Misconfigurations  
   5.2.2. Cron Job Exploitation  
   5.2.3. Kernel Exploits (e.g., Dirty COW)  
5.3. Exploiting Misconfigurations  
   5.3.1. File and Directory Permissions  
   5.3.2. Service Misconfigurations  

### Chapter 6: Defense Evasion
6.1. AMSI Bypass Techniques  
   6.1.1. PowerShell Obfuscation  
   6.1.2. DotNet AMSI Bypass  
   6.1.3. Inline C# Code Execution  
6.2. Obfuscation Techniques  
   6.2.1. Script and Binary Obfuscation  
6.3. Disabling Security Tools  
   6.3.1. Disabling EDR/AV Solutions  
   6.3.2. BYOVD (Bring Your Own Vulnerable Driver) Techniques  
6.4. Disabling and Deleting Logs  
   6.4.1. Avoid ETW Logging  
   6.4.2. Modifying or Deleting Logs  
6.5. Evasion Techniques  
   6.5.1. Fileless Malware Techniques  
   6.5.2. Living off the Land Binaries (LOLBins)  
   6.5.3. Using Fake Certificates to Sign Executables  
6.6. Process Injection and Hijacking  
   6.6.1. DLL Injection  
   6.6.2. Reflective DLL Injection  
   6.6.3. Remote Thread Injection  
   6.6.4. APC Injection  
   6.6.5. Thread Hijacking  
   6.6.6. PE Injection  
   6.6.7. IAT Hooking and Inline Hooking  
   6.6.8. Process Hollowing  
   6.6.9. Direct Syscalls  

### Chapter 7: Credential Access
7.1. Credential Dumping  
   7.1.1. Windows Credential Dumping  
   - Tools: Mimikatz, Rubeus, SharpHound  
   7.1.2. Techniques: NTLM Hash Extraction, Pass-the-Hash  
   7.1.3. Linux Credential Dumping  
   - Techniques: Extracting Passwords from Memory  
   7.1.4. Overview of LSASS Dump Techniques  
   - Techniques: Direct Dumping of LSASS Memory, Remote LSASS Dumping via PsExec, Lsassy (Rundll32.exe/comsvcs.dll)  
7.2. Pass-the-Hash and Pass-the-Ticket  
   7.2.1. NTLM Relay Attacks  
   7.2.2. Kerberos Ticket Attacks (Silver Ticket, Golden Ticket)  
7.3. Other Credential Access Techniques  
   7.3.1. Credential Harvesting from Web Browsers  
   7.3.2. Keylogging Techniques  

### Chapter 8: Pivoting and Lateral Movement
8.1. RDP, SMB, and WMI Exploitation  
   8.1.1. Using RDP for Lateral Movement  
   8.1.2. PsExec for Remote Command Execution  
   8.1.3. Leveraging SMB and WMI for Lateral Movement  
8.2. Tunneling Techniques to Move from a Subnet to Another  
   8.2.1. Tunneling  
   8.2.2. Socks Proxy  
8.3. Lateral Movement Tools and Techniques  
   8.3.1. PowerShell Remoting and WinRM  
   8.3.2. Custom Scripting for Lateral Movement  

### Chapter 9: Domain Escalation
9.1. AD Enumeration and Exploitation  
   9.1.1. ACLs in Active Directory  
   9.1.2. Locating and Enumerating Domain Admin Accounts  
   9.1.3. Mapping AD with BloodHound  
9.2. Exploiting Trust Relationships  
   9.2.1. Attack Paths via Trust Relationships  
9.3. Domain Controller Attacks  
   9.3.1. Kerberoasting, DCSync, DCShadow, and Other DC Exploits  
9.4. Gaining and Maintaining Domain Admin Access  
   9.4.1. Techniques for Persistence within the Domain  
9.5. Cross-Forest and Cross-Domain Escalation  
   9.5.1. Attacking Multiple Domains and Forests  

### Chapter 10: Command and Control (C2)
10.1. Setting Up C2 Infrastructure  
   10.1.1. Overview of C2 Tools  
   - Examples: Cobalt Strike, Empire, Covenant  
   10.1.2. Building a Resilient C2 Infrastructure  
   - Techniques: Domain Fronting, Redirectors  
10.2. Payload Development and AV Evasion  
   10.2.1. Obfuscation, Shellcode, Encoders  
   10.2.2. Bypassing EDR and AV with Custom Payloads  
10.3. C2 Communication Channels  
   10.3.1```markdown
### Chapter 10: Command and Control (C2)
10.1. Setting Up C2 Infrastructure  
   10.1.1. Overview of C2 Tools  
   - Examples: Cobalt Strike, Empire, Covenant  
   10.1.2. Building a Resilient C2 Infrastructure  
   - Techniques: Domain Fronting, Redirectors  
10.2. Payload Development and AV Evasion  
   10.2.1. Obfuscation, Shellcode, Encoders  
   10.2.2. Bypassing EDR and AV with Custom Payloads  
10.3. C2 Communication Channels  
   10.3.1. HTTP/S, DNS, and Custom Protocols  
   10.3.2. Steganography and Covert Channels for C2  
10.4. Advanced C2 Techniques  
   10.4.1. Steganography, Domain Fronting, Covert Channels  
   10.4.2. Managing C2 in Complex Environments  
10.5. Case Study: Real-World C2 Operations  
   10.5.1. Analysis of High-Profile C2 Scenarios  

### Chapter 11: Data Exfiltration
11.1. Data Exfiltration Over Common Protocols  
   11.1.1. HTTP, HTTPS, and DNS Tunneling Techniques  
   11.1.2. Leveraging Cloud Services for Exfiltration  
11.2. Covert Data Exfiltration  
   11.2.1. Exfiltrating Data Over Non-Traditional Channels  
   11.2.2. Encryption and Steganography for Data Exfiltration  

### Chapter 12: Post-Exploitation and Reporting
12.1. Maintaining Access  
   12.1.1. Techniques for Long-Term Persistence  
   12.1.2. Cleanup and Avoiding Detection  
12.2. Evidence Gathering and Reporting  
   12.2.1. Collecting Evidence and Artifacts  
   12.2.2. Crafting a Comprehensive Red Team Report  
12.3. Lessons Learned and Remediation Recommendations  
   12.3.1. Analyzing Gaps and Strengthening Defenses  
   12.3.2. Collaborating with Blue Teams for Defense Improvements  

### Chapter 13: Advanced Red Teaming Scenarios
13.1. Real-World Red Team Case Studies  
   13.1.1. Analysis of High-Profile Red Team Operations  
   13.1.2. Lessons Learned from Notable Engagements  
13.2. Continuous Red Team Operations  
   13.2.1. Long-Term Engagements and Red Team/Blue Team Collaboration  
   13.2.2. Continuous Improvement and Adversary Simulation Updates  
