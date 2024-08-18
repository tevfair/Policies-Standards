
# Cloud / DevSecOps Security Standards: Development, IaC, and CI/CD

| Version | Author         | Description                       | Date      |
|---------|----------------|-----------------------------------|-----------|
| 1.0     | Tevin Fair  | Initial publication |08/11/2024 |

---

### Standard 800 - 01: Code Repository Security

- **Description**: Establish robust security for source code repositories to protect against unauthorized access and changes.
- **Policy Mapping**:
  - Policy 900 - 01: Code Repository Security
- **CIS Mapping**:
  - CIS Control: 5.1, 5.2 (Secure Repository Access and Audit Logging)
- **CSA CCM Mapping**:
  - CSA CCM: MOB-01, DAC-02 (Mobile Device Management and Data Access Monitoring)
- **Implementation**:
  - Ensure repositories are private by default.
  - Implement role-based access control for repositories.
  - Enable detailed logging of all access and change events.
  - Conduct regular audits of repository access logs.
  - Enforce two-factor authentication (2FA) for repository access.

---

### Standard 800 - 02: Secure Software Development Life Cycle (SDLC)

- **Description**: Incorporate security considerations and checks throughout the SDLC.
- **Policy Mapping**:
  - Policy 900 - 02: Secure Software Development Life Cycle (SDLC)
- **CIS Mapping**:
  - CIS Control: 6.1, 6.2 (SDLC Security Integration and Secure Coding Training)
- **CSA CCM Mapping**:
  - CSA CCM: STA-08, TRA-01 (Static Code Analysis and Security Awareness Training)
- **Implementation**:
  - Integrate security reviews and vulnerability assessments into each phase of the SDLC.
  - Deliver recurring training sessions on secure coding practices to development teams.

---

### Standard 800 - 03: Version Control for IaC

- **Description**: Ensure proper versioning for all Infrastructure as Code (IaC) configurations.
- **Policy Mapping**:
  - Policy 900 - 03: Version Control
- **CIS Mapping**:
  - CIS Control: 7.2, 7.3 (IaC Version Control and Historical Version Retention)
- **CSA CCM Mapping**:
  - CSA CCM: IVM-04, DCS-05 (Vulnerability/Patch Management and Data Security/Integrity)
- **Implementation**:
  - Maintain all IaC configurations in version-controlled systems.
  - Preserve historical versions of configurations in line with compliance mandates.

---

### Standard 800 - 04: Configuration Validation for IaC

- **Description**: Authenticate and scrutinize IaC configurations to prevent security misconfigurations before implementation.
- **Policy Mapping**:
  - Policy 900 - 04: Configuration Validation
- **CIS Mapping**:
  - CIS Control: 7.5, 7.6 (IaC Pre-Validation and Static Analysis for Misconfigurations)
- **CSA CCM Mapping**:
  - CSA CCM: GRM-01, DCS-04 (Governance/Risk Management and Data Security)
- **Implementation**:
  - Check configurations against security best practices prior to applying IaC changes.
  - Employ automated tools to conduct static analysis on IaC templates to uncover potential vulnerabilities.

---

### Standard 800 - 05: Least Privilege Principle in IaC

- **Description**: Adhere to the principle of least privilege when setting permissions in IaC configurations.
- **Policy Mapping**:
  - Policy 900 - 05: Least Privilege Principle
- **CIS Mapping**:
  - CIS Control: 4.2 (Least Privilege Implementation)
- **CSA CCM Mapping**:
  - CSA CCM: ACC-03 (Access Control)
- **Implementation**:
  - Assign only indispensable permissions within IaC configurations.
  - Periodically review and refine permissions to minimize potential exposure.

---

### Standard 800 - 06: Secrets Management in IaC

- **Description**: Guard against embedding sensitive information within IaC scripts and ensure secured storage.
- **Policy Mapping**:
  - Policy 900 - 06: Secrets Management
- **CIS Mapping**:
  - CIS Control: 13.3, 13.4 (Sensitive Data Protection and Encrypted Storage)
- **CSA CCM Mapping**:
  - CSA CCM: SEC-02, SEC-03 (Secure Data Handling and Encrypted Storage)
- **Implementation**:
  - Avoid embedding sensitive data such as API keys or passwords directly in IaC scripts.
  - Utilize dedicated secrets management solutions or encrypted storage mechanisms for sensitive information.

---

### Standard 800 - 07: Automated Security Testing in CI/CD

- **Description**: Integrate automated security testing mechanisms within CI/CD pipelines to continually assess for potential vulnerabilities.
- **Policy Mapping**:
  - Policy 900 - 07: Automated Security Testing
- **CIS Mapping**:
  - CIS Control: 18.1, 18.2 (Automated Security Testing Integration and Dependency Scanning)
- **CSA CCM Mapping**:
  - CSA CCM: SAM-02, SAM-03 (Security Testing/Scanning and Secure Build Process)
- **Implementation**:
  - Embed automated security testing solutions within CI/CD processes.
  - Conduct recurring scans of the codebase and its dependencies for potential vulnerabilities.

---

### Standard 800 - 08: Dependency Management in CI/CD

- **Description**: Ensure that all software dependencies are regularly checked for vulnerabilities and kept up-to-date.
- **Policy Mapping**:
  - Policy 900 - 08: Dependency Management
- **CIS Mapping**:
  - CIS Control: 3.4, 3.5 (Dependency Vulnerability Scanning and Outdated Dependency Replacement)
- **CSA CCM Mapping**:
  - CSA CCM: SAM-04, SAM-05 (Security Patch Management and Vulnerability Management)
- **Implementation**:
  - Use automated solutions to continuously check dependencies for recognized security vulnerabilities.
  - Act promptly to update or replace any outdated or vulnerable software dependencies.

---

### Standard 800 - 09: Immutable Infrastructure

- **Description**: Promote the adoption of immutable infrastructure where resources are not altered post-deployment but replaced with new versions.
- **Policy Mapping**:
  - Policy 900 - 09: Immutable Infrastructure
- **CIS Mapping**:
  - CIS Control: 8.4 (Immutable and Version Controlled Configurations)
- **CSA CCM Mapping**:
  - CSA CCM: DCS-08 (Data Integrity and Security)
- **Implementation**:
  - Aim to construct an environment where once resources are deployed, modifications are prohibited.
  - Any change or update should result in a new resource version, rather than altering the existing one.

---

### Standard 800 - 10: Access Control for CI/CD tools

- **Description**: Implement strict access control mechanisms for CI/CD tools, maintaining thorough logs for all activities.
- **Policy Mapping**:
  - Policy 900 - 10: Access Control
- **CIS Mapping**:
  - CIS Control: 4.3, 4.4 (Restrict Access to CI/CD tools and Audit Log Maintenance)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-12, IAM-13 (User Access Restriction and Logging)
- **Implementation**:
  - Limit CI/CD tool access to essential and authorized personnel only.
  - Ensure comprehensive logs are maintained for all CI/CD tool activities.

---

### Standard 800 - 11: Secure Artifact Management

- **Description**: Artifacts generated during the build process must be stored securely in controlled repositories, ensuring their integrity.
- **Policy Mapping**:
  - Policy 900 - 11: Artifact Management
- **CIS Mapping**:
  - CIS Control: 8.7, 8.8 (Secure Artifact Storage and Integrity Verification)
- **CSA CCM Mapping**:
  - CSA CCM: DSI-02, DSI-03 (Data Storage and Integrity)
- **Implementation**:
  - Store build artifacts in secure, access-controlled repositories.
  - Validate and authenticate artifact integrity before deployment.

---

### Standard 800 - 12: Production and Non-Production Environment Isolation

- **Description**: Establish a clear demarcation between production and non-production environments. Ensure direct deployments don't occur to production without passing through appropriate stages.
- **Policy Mapping**:
  - Policy 900 - 12: Environment Isolation
- **CIS Mapping**:
  - CIS Control: 7.9, 7.10 (Environment Separation and Deployment Process)
- **CSA CCM Mapping**:
  - CSA CCM: SEF-01, SEF-02 (Production / Non-production Segregation)
- **Implementation**:
  - Design and implement strict boundaries between production and non-production environments.
  - Ensure deployments to production are performed only after adequate testing and approval in staging or equivalent environments.

---
