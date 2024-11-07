# Forage-Internship-AIG
A quick description of what I did in Forage Internship. It was mainly focused on learning about Log4j vulnerability and advising how to mitigate it. In the second part of the internship I had to conduct a brute-force attack on encrypted files.

# AIG’s Shields Up: Cybersecurity Job Simulation!

### Role: Information Security Analyst in the Cyber & Information Security Team

As an Information Security Analyst, one of your primary responsibilities is to stay ahead of emerging vulnerabilities to help prevent potential security breaches. In this task, you'll review critical information on two recent advisories published by the Cybersecurity & Infrastructure Security Agency (CISA) and draft a security advisory email regarding the Apache Log4j vulnerability.

---

## Task 1: Review of CISA Advisories

![obraz](https://github.com/user-attachments/assets/d6f62584-f46a-4194-8b84-fcf8eca9cbb2)


### CISA's Recent Advisories
1. **Apache Log4j Vulnerability (Log4Shell)**: A critical vulnerability in a widely-used Java-based logging library.
2. **Ransomware Trends**: Highlights the rise and professionalization of ransomware attacks—a concern for large enterprises like AIG.

### Key Findings on Log4j Vulnerability
- **Severity**: Apache has classified vulnerabilities such as Log4Shell (CVE-2021-44228) as critical and CVE-2021-45046 as high-risk.
- **Exploitation Risks**: An attacker can take control of a vulnerable system, enabling activities such as data theft, ransomware deployment, and further system compromise.
- **Mitigation Recommendations**:
  - Identify and patch assets using Log4j to the latest version.
  - Inventory and monitor assets, ensuring updates reach all users.
  - Implement threat detection and incident response to monitor any signs of exploitation.

![obraz](https://github.com/user-attachments/assets/cc5e7144-dc9c-46cc-933b-3682aaf6a0f8)


### Drafted Advisory Email

**From**: AIG Cyber & Information Security Team  
**To**: product@email.com  
**Subject**: Security Advisory concerning Apache Log4j Vulnerability

**Body**:
> Hello John Doe,  
>  
> The AIG Cyber & Information Security Team would like to inform you of a critical vulnerability affecting systems using the Apache Log4j logging library. This vulnerability, known as Log4Shell (CVE-2021-44228), along with CVE-2021-45046, poses a severe risk to infrastructure that relies on Log4j, commonly found in enterprise applications and systems.  
>  
> **Vulnerability Description**  
> Log4Shell and related vulnerabilities allow attackers to execute arbitrary code remotely, which can lead to full system control and enable malicious actions, such as data theft or ransomware deployment.  
>  
> **Risk and Impact**  
> Given the widespread use of Java and the ease of exploitation, this vulnerability is highly critical. Unpatched systems are especially vulnerable, as adversaries could exploit them to access sensitive data and disrupt operations.  
>  
> **Remediation Steps**  
> - **Upgrade Log4j**:  
>   - For systems running Java 8 or later, update Log4j to version 2.17.0 or newer.  
>   - For Java 7 environments, update to Log4j version 2.12.3.  
> - **Inventory and Patch Vulnerable Assets**:  
>   - Identify all assets using Log4j, apply the latest patches, and track these assets carefully to avoid potential exploitation.  
>   - Use tools such as CISA's GitHub repository and CERT/CC’s CVE-2021-44228 scanner to locate any susceptible assets.  
> - **Initiate Threat Hunts**:  
>   - Treat any unpatched Log4j assets as potentially compromised. Conduct forensic analysis, monitor connected accounts, and verify all configuration changes since December 1, 2021.  
>  
> **Confirmation of Action**  
> Please confirm once these mitigations have been completed. This will ensure we maintain a high level of security across our infrastructure. For further assistance, don’t hesitate to reach out to us.  
>  
> Kind regards,  
> AIG Cyber & Information Security Team

---

## Task 2: Incident Response – Brute-forcing the Encryption Key

Despite the advisory email, an attacker managed to exploit the Log4j vulnerability, initiating a ransomware attack. Fortunately, the Incident Detection & Response team prevented complete ransomware installation, limiting encryption to a single zip file. The Chief Information Security Officer (CISO) has decided not to pay the ransom, given the risk of re-encryption or future attacks.

### Task Objective
Your next task is to bruteforce the decryption key, given the attacker’s apparent lack of sophistication in encryption methods.

This is how the folder structure looked like:

![obraz](https://github.com/user-attachments/assets/b9101fbd-1217-4e6d-a8c4-7ba02995a4b6)

Below is the script created to begin the brute-force process:

![obraz](https://github.com/user-attachments/assets/3e6febff-174f-4485-9825-977e81803e01)

And the succesful attempt:

![obraz](https://github.com/user-attachments/assets/1b1d74f1-5ec1-45ea-8a1f-e2990dbc5cc2)

---

> **Certification**  
> For more information on my certification related to this simulation, view it here:  
> [Completion Certificate](https://forage-uploads-prod.s3.amazonaws.com/completion-certificates/4nAmAbTbHbnGMNSyo/2ZFnEGEDKTQMtEv9C_4nAmAbTbHbnGMNSyo_Z3Nsom8sbe2WPduza_1730924838043_completion_certificate.pdf)
