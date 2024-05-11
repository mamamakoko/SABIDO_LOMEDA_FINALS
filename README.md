## Ethical Hacking Technical Report
**Client:	Nestlé Philippines (nestle.com.ph)**  
**Date:	May 10, 2024**  
**Prepared by:	Crizzalie M. Sabido and John Francis B. Lomeda**  

**Executive Summary:** This report presents the technical findings of the ethical hacking assessment conducted for Nestlé Philippines (nestle.com.ph). The assessment aimed to identify vulnerabilities within the organization's network infrastructure, applications, and systems. Through various testing methodologies, including penetration testing and vulnerability scanning, critical and high-risk issues were discovered. This report provides detailed descriptions of these findings, along with actionable recommendations for 
remediation.
___
**Vulnerability Summary:**  
- **R00TK1T Attack (April 2024)**:

  - **Critical**: Successful infiltration of Nestlé’s systems, potentially exposing them to remote exploitation and potential network compromise.
  - **High**: Exposure of confidential data, increasing the risk of unauthorized access to sensitive information.

- **Data Breach (March 2022)**:

  -   **Critical**: Significant data breach attributed to the hacktivist group known as Anonymous.
  -   **High**: Disclosure of a substantial 10GB trove of data, including sensitive information such as emails, passwords, and client data.

- **Network Infrastructure:**
  - **Critical:** Unpatched firmware in network switches, exposing them to remote exploitation and potential network compromise.
  - **High:** Inadequate network segmentation allowing lateral movement within the network, increasing the risk of unauthorized access to sensitive data.

- **Web Applications:**
  - **Critical:** Lack of input validation in the user registration form, leading to potential injection attacks and unauthorized access to the application backend.
  - **High:** Insecure direct object references (IDOR) in the application, allowing attackers to access restricted resources by manipulating parameters in requests.

- **Operating Systems:**
  - **Critical:** End-of-life (EOL) operating systems (e.g., Windows 7) on employee workstations, leaving them vulnerable to known exploits and malware.
  - **High:** Insufficient logging and monitoring on critical servers, hindering the detection of suspicious activities and potential security breaches.

- **Wireless Networks:**
  - **Critical:** Default credentials used in wireless access points, enabling unauthorized individuals to gain access to the network infrastructure.
  - **High:** Lack of intrusion detection and prevention systems (IDPS) in wireless networks, making it difficult to detect and respond to wireless attacks.

- **Social Engineering:**
  - **High:** Employees sharing sensitive information over unencrypted channels (e.g., email), increasing the risk of data leakage and unauthorized access.

- **Physical Security**:
  -   **Critical**: Inadequate surveillance in server rooms, increasing the risk of unauthorized physical access to critical infrastructure.
  -   **High**: Insufficient access controls for secure areas, potentially allowing unauthorized personnel access to sensitive areas.

- **User Awareness and Training**:

  -   **High**: Employees not trained on cybersecurity best practices, increasing the risk of successful social engineering attacks.

- **Database Systems**:

  -   **Critical**: Use of default database credentials, enabling unauthorized individuals to gain access to sensitive data.
  -   **High**: Lack of encryption for data at rest, increasing the risk of data exposure in the event of a breach.
___
**Recommendations:**

-   **R00TK1T Attack (April 2024)**:
    
    -   **Critical**: Implement  **intrusion detection systems (IDS)**  and  **intrusion prevention systems (IPS)**  to detect and prevent future infiltrations. Regularly update these systems to recognize the latest threats.
    -   **High**: Establish a  **data classification policy**  to identify and protect confidential data. Use encryption, access controls, and regular audits to ensure data is only accessible to authorized individuals.
-   **Data Breach (March 2022)**:
    
    -   **Critical**: Conduct a thorough  **incident response investigation**  to understand the breach’s full extent and prevent similar incidents in the future. This could involve hiring a third-party cybersecurity firm.
    -   **High**: Notify affected parties of the breach and offer support such as credit monitoring services. Implement  **data loss prevention (DLP) tools**  to monitor and protect sensitive data. Regularly review and update these tools to align with the latest threats and regulatory requirements.
- **Network Infrastructure:**
  - Immediately update firmware on all network switches to mitigate known vulnerabilities and enhance network security.
Implement network segmentation to restrict lateral movement and isolate critical assets from unauthorized access.

- **Web Applications:**
  - Enhance input validation mechanisms in the user registration form to prevent injection attacks and ensure the integrity of user data.
Implement access controls and proper authorization mechanisms to mitigate the risk of IDOR vulnerabilities.

- **Operating Systems:**
  - Upgrade EOL operating systems to supported versions or implement compensating controls to mitigate the associated risks.
Deploy robust logging and monitoring solutions on critical servers to enhance visibility into network activities and detect potential security incidents.

- **Wireless Networks:**
  - Change default credentials on wireless access points and enforce strong authentication mechanisms to prevent unauthorized access.
Implement IDPS in wireless networks to detect and prevent malicious activities, such as rogue access points and reauthentication attacks.

- **Social Engineering:**
  - Educate employees on the importance of using secure communication channels for sharing sensitive information and provide training on identifying social engineering attacks.
Implement encryption protocols (e.g., TLS) for email communications to protect sensitive data from interception and unauthorized access.

-   **Physical Security**:
    
    -   **Critical**: Implement a  **surveillance system**  in server rooms, such as CCTV cameras, to monitor and record activities. This will deter unauthorized access and provide evidence in case of security incidents.
    -   **High**: Establish  **strict access controls**  for secure areas. This could include key card access systems, biometric scanners, or manned security checkpoints to ensure only authorized personnel can enter sensitive areas.
-   **User Awareness and Training**:
    
    -   **High**: Conduct regular  **cybersecurity training sessions**  for all employees. This should cover topics like recognizing phishing attempts, secure password practices, and the importance of not sharing sensitive information. Regularly test employees with simulated attacks to reinforce learning and identify areas for improvement.
-   **Database Systems**:
    
    -   **Critical**: Change all  **default database credentials**  immediately after installation and regularly thereafter. Use strong, unique passwords and consider implementing multi-factor authentication for added security.
    -   **High**: Implement  **encryption for data at rest**. This ensures that even if data is accessed, it cannot be read without the encryption key. Regularly review and update encryption methods to align with industry best practices.
