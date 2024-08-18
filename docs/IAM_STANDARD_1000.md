# Cloud Security Standards: Identity and Access Management (IAM)

| Version | Author         | Description                       | Date      |
|---------|----------------|-----------------------------------|-----------|
| 1.0     | Tevin Fair  | Initial publication |08/11/2024 |

---

### Standard - 1000 - 01: User Onboarding

- **Description**: Ensure that users undergo a stringent vetting process prior to being granted access to cloud resources.
- **Policy Mapping**:
  - Policy 1000 - 01: User Onboarding
- **CIS Mapping**:
  - CIS Control: 16.5 (Account Monitoring and Control)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-01 (User Identity Management)
- **Implementation**:
  - Implement rigorous user identity verification mechanisms using valid documentation.
  - Ensure that access levels granted are pertinent to the user's role.
  - Continuously reassess and refine onboarding processes to account for changing requirements.

---

### Standard - 1000 - 02: User Off-boarding

- **Description**: Terminate access rights promptly upon employment cessation or role change.
- **Policy Mapping**:
  - Policy 1000 - 02: User Off-boarding
- **CIS Mapping**:
  - CIS Control: 16.6 (Account Termination Process)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-02 (User Access Reviews & Revocation)
- **Implementation**:
  - Foster collaboration with HR to ensure swift access termination.
  - Maintain an activity log for off-boarded users to monitor any post-termination actions.

---

### Standard - 1000 - 03: Session Timeouts

- **Description**: Ensure that inactive sessions are automatically terminated after a defined period.
- **Policy Mapping**:
  - Policy 1000 - 05: Session Timeouts
- **CIS Mapping**:
  - CIS Control: 16.9 (Session Lock with Pattern-Hiding Displays)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-07 (Session Time-out)
- **Implementation**:
  - Enforce a mandatory session timeout, especially within high-security environments.
  - Regularly review and adjust the duration of session timeouts based on the risk assessment.

---

### Standard - 1000 - 04: Least Privilege Access

- **Description**: Ensure that users are provided the minimal amount of access necessary to complete their tasks.
- **Policy Mapping**:
  - Policy 1000 - 07: Least Privilege
- **CIS Mapping**:
  - CIS Control: 4.3 (Control Use of Administrative Privileges)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-03 (User Access Reviews & Revocation)
- **Implementation**:
  - Implement strict role-based access controls (RBAC) to restrict permissions.
  - Perform regular audits to detect and rectify any instances of excessive permissions.

---

### Standard - 1000 - 05: Data Encryption

- **Description**: Mandate the encryption of data, both at rest and during transit.
- **Policy Mapping**:
  - Policy 1000 - 10: Data Encryption
- **CIS Mapping**:
  - CIS Control: 13.1 (Maintain an Inventory of Cryptographic Material)
- **CSA CCM Mapping**:
  - CSA CCM: DCS-01 (Data Encryption & Tokenization)
- **Implementation**:
  - Implement AES-256 encryption or other industry-recognized encryption methods.
  - Regularly review and update encryption protocols to match industry advancements.

---

### Standard - 1000 - 06: Data Sharing and Authorization

- **Description**: Establish protocols to ensure data isn't shared without proper authorization and audit trails.
- **Policy Mapping**:
  - Policy 1000 - 11: Data Sharing
- **CIS Mapping**:
  - CIS Control: 13.2 (Protect Information Through Access Controls)
- **CSA CCM Mapping**:
  - CSA CCM: DCS-04 (Secure Data Transfer & Storage)
- **Implementation**:
  - Adhere to internal and regulatory standards for data sharing.
  - Ensure secure channels are used when sharing, and encrypt data during transfer.

---

### Standard - 1000 - 07: Data Retention and Disposal

- **Description**: Clearly define and enforce data retention periods and ensure secure disposal of data.
- **Policy Mapping**:
  - Policy 1000 - 12: Data Retention
  - Policy 1000 - 14: Data Disposal
- **CIS Mapping**:
  - CIS Control: 11.6 (Securely Store Master Images)
  - CIS Control: 11.7 (Securely Dispose of or Reuse Equipment)
- **CSA CCM Mapping**:
  - CSA CCM: DSI-04 (Data Ownership/ Stewardship)
- **Implementation**:
  - Regularly review data and delete any information past its retention period or no longer necessary.
  - Employ certified tools or services to securely dispose of data and ensure it meets industry standards.

---

### Standard - 1000 - 08: Data Backups and Recovery

- **Description**: Regularly back up critical data and test its recovery to ensure business continuity.
- **Policy Mapping**:
  - Policy 1000 - 13: Data Backups
- **CIS Mapping**:
  - CIS Control: 10.5 (Ensure Regular Data Backups)
- **CSA CCM Mapping**:
  - CSA CCM: BCR-01 (Backup and Restoration Policy & Procedures)
- **Implementation**:
  - Store backups in secure locations with restricted access.
  - Periodically test backup recovery procedures to confirm the integrity of the data and ensure quick recovery times.

---

### Standard - 1000 - 09: Data Masking in Non-Production Environments

- **Description**: Ensure that sensitive data is appropriately masked in test, development, and other non-production environments.
- **Policy Mapping**:
  - Policy 1000 - 15: Data Masking
- **CIS Mapping**:
  - CIS Control: 14.3 (Protect Sensitive Information in Non-Production Environments)
- **CSA CCM Mapping**:
  - CSA CCM: DSI-02 (Data Handling/Labeling/Security Policy)
- **Implementation**:
  - Implement data anonymization techniques to obscure sensitive data.
  - Review and restrict access to non-production environments to further reduce exposure risks.

---

### Standard - 1000 - 10: Data Breach Preparedness and Response

- **Description**: Establish a clear and documented plan to handle potential data breaches.
- **Policy Mapping**:
  - Policy 1000 - 16: Data Breach Response
- **CIS Mapping**:
  - CIS Control: 19.7 (Incident Response Management Plan)
- **CSA CCM Mapping**:
  - CSA CCM: IRM-02 (Incident Reporting)
- **Implementation**:
  - Ensure all personnel are familiar with the data breach response plan.
  - Regularly test and update the plan using simulated incidents to evaluate and improve response times and effectiveness.

---

### Standard - 1000 - 11: Data Access Monitoring and Logging

- **Description**: Log and monitor all access and modifications to critical data.
- **Policy Mapping**:
  - Policy 1000 - 17: Data Access Logs
- **CIS Mapping**:
  - CIS Control: 6.2 (Activate audit logging)
- **CSA CCM Mapping**:
  - CSA CCM: GRM-01 (Baseline Requirements)
- **Implementation**:
  - Ensure logs are comprehensive and capture all necessary information.
  - Store logs securely and in a tamper-evident environment.

---

### Standard - 1000 - 12: Data Integrity Verification

- **Description**: Regularly verify the integrity and consistency of stored data.
- **Policy Mapping**:
  - Policy 1000 - 18: Data Integrity Checks
- **CIS Mapping**:
  - CIS Control: 8.2 (Integrity Checking Mechanisms)
- **CSA CCM Mapping**:
  - CSA CCM: DSI-01 (Data Security/Integrity)
- **Implementation**:
  - Utilize checksums, hashes, and other data verification methods to maintain data integrity.
  - Schedule regular checks to ensure data consistency and address any discrepancies.

---

### Standard - 1000 - 13: User Access Vetting and Authorization

- **Description**: Ensure a thorough process for vetting and authorizing user access to cloud resources.
- **Policy Mapping**:
  - Policy 1000 - 01: User Onboarding
  - Policy 1000 - 02: User Off-boarding
  - Policy 1000 - 03: Periodic User Review
  - Policy 1000 - 04: Role Change
- **CIS Mapping**:
  - CIS Control: 16.7 (User Access Reviews)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-03 (User Access Reviews/Re-certifications)
- **Implementation**:
  - Collaborate with HR and department heads to verify user identity and necessity of access.
  - Implement automated tools for immediate revocation of access rights upon employment changes.
  - Schedule quarterly reviews of user access and roles.

---

### Standard - 1000 - 14: Session Security

- **Description**: Enhance security during user sessions.
- **Policy Mapping**:
  - Policy 1000 - 05: Session Timeouts
  - Policy 1000 - 06: Concurrent Sessions
- **CIS Mapping**:
  - CIS Control: 4.5 (Use Session Lock With Inactivity Timeout)
  - CIS Control: 16.2 (Account Inactivity Timeout)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-08 (Session Locking)
- **Implementation**:
  - Set a 15-minute inactivity timeout for high-security sessions.
  - Restrict users to a single active session to prevent potential misuse.

---

### Standard - 1000 - 15: Service Access Restrictions

- **Description**: Ensure users have access only to necessary services and regions.
- **Policy Mapping**:
  - Policy 1000 - 07: Least Privilege
  - Policy 1000 - 08: Service Restrictions
  - Policy 1000 - 09: Temporary Access
- **CIS Mapping**:
  - CIS Control: 4.3 (Separation of Duties of Privileged Functions)
  - CIS Control: 14.6 (Least Privilege)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-10 (Privileged User Access Restriction)
- **Implementation**:
  - Adopt the principle of least privilege across all cloud services.
  - Block unnecessary services or regions by default and review permissions regularly.
  - Ensure all temporary access requests are documented and time-bound.

---

### Standard - 1000 - 16: Data Security Best Practices

- **Description**: Implement best practices to secure data throughout its lifecycle.
- **Policy Mapping**:
  - Policy 1000 - 10: Data Encryption
  - Policy 1000 - 15: Data Masking
  - Policy 1000 - 16: Data Breach Response
  - Policy 1000 - 17: Data Access Logs
  - Policy 1000 - 18: Data Integrity Checks
- **CIS Mapping**:
  - CIS Control: 13.1 (Maintain an Inventory of Sensitive Information)
  - CIS Control: 13.6 (Protect Sensitive Information in Shared Environments)
- **CSA CCM Mapping**:
  - CSA CCM: DSI-05 (Data Security/Protection Lifecycle)
- **Implementation**:
  - Enforce encryption standards for data at rest and in transit.
  - Implement data masking techniques for sensitive data in non-production environments.
  - Monitor logs for unauthorized data access and ensure integrity checks.

---
