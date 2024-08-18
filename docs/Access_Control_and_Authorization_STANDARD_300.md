# Cloud Security Standard: Access Control and Authorization

| Version | Author         | Description                       | Date      |
|---------|----------------|-----------------------------------|-----------|
| 1.0     | Tevin Fair  | Initial publication |08/11/2024 |

---

### Standard - 300 - 01: Role Definition and Assignment

- **Description**: Define and allocate roles grounded in organizational responsibilities, ensuring cloud resources' access aligns with these roles.
- **Policy Mapping**:
  - Policy 300 - 01: Define and Assign Roles
- **CIS Mapping**:
  - CIS Control: 16 (Account Monitoring and Control)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-02 (User Access Policy)
- **Implementation**:
  - Use cloud-native IAM solutions to define and assign roles.
  - Regularly review role definitions to keep them current.

---

### Standard - 300 - 02: Duty Segregation

- **Description**: Ensure responsibilities are adequately distributed to prevent undue control over critical transactions by a single individual.
- **Policy Mapping**:
  - Policy 300 - 02: Segregation of Duties
- **CIS Mapping**:
  - CIS Control: 4 (Controlled Use of Administrative Privileges)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-05 (Source Code Access Restriction)
- **Implementation**:
  - Design workflows requiring multi-person approval for sensitive tasks.
  - Monitor for potential breaches of this principle.

---

### Standard - 300 - 03: Apply Least Privilege

- **Description**: Grant only essential permissions, minimizing excessive access.
- **Policy Mapping**:
  - Policy 300 - 03: Least Privilege Principle
- **CIS Mapping**:
  - CIS Control: 14 (Controlled Access Based on the Need to Know)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-01 (User Access Management)
- **Implementation**:
  - Periodically review permissions, revoking unnecessary ones.
  - Utilize tools to analyze effective permissions.

---

### Standard - 300 - 04: Periodic Access Verification

- **Description**: Regularly validate that users possess appropriate access rights.
- **Policy Mapping**:
  - Policy 300 - 04: Regular Access Audits
- **CIS Mapping**:
  - CIS Control: 16 (Account Monitoring and Control)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-06 (User Access Reviews)
- **Implementation**:
  - Schedule quarterly access reviews.
  - Use automated tools for large-scale access evaluations.

---

### Standard - 300 - 05: Leadership Access Endorsement

- **Description**: Ensure that leadership regularly certifies the access rights of their teams.
- **Policy Mapping**:
  - Policy 300 - 05: Certification of Access
- **CIS Mapping**:
  - CIS Control: 16 (Account Monitoring and Control)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-06 (User Access Reviews)
- **Implementation**:
  - Use automated workflow tools to manage access endorsement cycles.
  - Track non-compliance and escalate as necessary.

---

### Standard - 300 - 06: Conditional Elevated Access

- **Description**: Grant heightened access under specific conditions and for limited durations.
- **Policy Mapping**:
  - Policy 300 - 06: Temporary Elevation
- **CIS Mapping**:
  - CIS Control: 4 (Controlled Use of Administrative Privileges)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-08 (User Access Revocation)
- **Implementation**:
  - Implement JIT protocols for requesting elevated access.
  - Automate de-escalation post-task or after a set duration.

---

### Standard - 300 - 07: Precise Administrative Access

- **Description**: Equip administrators with only the access level necessary for their tasks.
- **Policy Mapping**:
  - Policy 300 - 07: Just-Enough-Administration
- **CIS Mapping**:
  - CIS Control: 4 (Controlled Use of Administrative Privileges)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-03 (User Access Settings)
- **Implementation**:
  - Categorize administrative tasks, granting access accordingly.
  - Train administrators on the importance of this principle.

---

### Standard - 300 - 08: Supervise JIT and JEA Activities

- **Description**: Monitor all JIT and JEA actions, alerting on anomalies.
- **Policy Mapping**:
  - Policy 300 - 08: Logging and Monitoring JIT and JEA
- **CIS Mapping**:
  - CIS Control: 6 (Maintenance, Monitoring, and Analysis of Audit Logs)
- **CSA CCM Mapping**:
  - CSA CCM: SEF-01 (Audit Logging / Intrusion Detection)
- **Implementation**:
  - Integrate JIT and JEA actions with SIEM solutions.
  - Regularly review and refine monitoring
### Standard - 300 - 09: Role-Based Access Control Configuration

- **Description**: Implement and enforce RBAC to manage access to cloud resources.
- **Policy Mapping**:
  - Policy 300 - 01: Define and Assign Roles
  - Policy 300 - 02: Segregation of Duties
  - Policy 300 - 03: Least Privilege Principle
- **CIS Mapping**:
  - CIS Control: 1.4 (Maintain an Inventory of Administrative Accounts)
  - CIS Control: 1.6 (Use Dedicated Administrative Accounts)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-04 (User Access Restriction/Authorization)
- **Implementation**:
  - Regularly review and update RBAC configurations to ensure alignment with the current organizational structure.
  - Integrate RBAC with central identity providers.

---

### Standard - 300 - 10: Access Review and Remediation

- **Description**: Implement regular access reviews, ensuring users and roles are in line with current organizational requirements.
- **Policy Mapping**:
  - Policy 300 - 04: Regular Access Audits
  - Policy 300 - 05: Certification of Access
- **CIS Mapping**:
  - CIS Control: 16.2 (Account Monitoring)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-07 (User Access Recertification)
- **Implementation**:
  - Use automated tools to track role and access changes.
  - Develop procedures for remediation when discrepancies are found.

---

### Standard - 300 - 11: Temporary and Elevated Access Management

- **Description**: Control and monitor temporary and elevated access requests and usage.
- **Policy Mapping**:
  - Policy 300 - 06: Temporary Elevation
  - Policy 300 - 07: Just-Enough-Administration
  - Policy 300 - 08: Logging and Monitoring JIT and JEA
- **CIS Mapping**:
  - CIS Control: 4.2 (Change Administrative Credentials)
  - CIS Control: 4.3 (Use Dedicated Administrative Accounts)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-10 (User ID Credential Policy)
- **Implementation**:
  - Ensure proper documentation of all elevated access requests.
  - Regularly review JIT and JEA logs for misuse or potential policy violations.

---

### Standard - 300 - 12: Identity and Access Governance

- **Description**: Establish a governance framework for identity and access to ensure compliance and ongoing alignment with organizational needs.
- **Policy Mapping**:
  - Policy 300 - 01: Define and Assign Roles
  - Policy 300 - 04: Regular Access Audits
  - Policy 300 - 05: Certification of Access
- **CIS Mapping**:
  - CIS Control: 16.6 (Account Use Confirmation)
- **CSA CCM Mapping**:
  - CSA CCM: IAM-09 (Third Party Access)
- **Implementation**:
  - Establish a committee or working group dedicated to access governance.
  - Develop a lifecycle management process for identities, roles, and access permissions.