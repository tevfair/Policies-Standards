# Cloud Network Security Standards with CIS & CSA CCM Mapping

| Version | Author         | Description                       | Date      |
|---------|----------------|-----------------------------------|-----------|
| 1.0     | Tevin Fair  | Initial publication |08/11/2024 |

---

## Network Security Standards

### Standard 700 - 01: Least Privilege Architecture

- **Description**: Implement architectures that adhere to the least privilege principle.
- **Policy Mapping**:
  - Policy 700 - 01: Design
- **CIS Mapping**:
  - CIS Control: 14.6 (Segmentation and Segregation)
- **CSA CCM Mapping**:
  - CSA CCM: DSI-02 (Data Ownership)
- **Implementation**:
  - Use isolated VPCs/Vnets for each business unit or application.
  - Implement network segmentation based on workloads and sensitivity of the data.

---

### Standard 700 - 02: Geographical Resource Management

- **Description**: Distribute cloud resources across multiple regions to ensure high availability.
- **Policy Mapping**:
  - Policy 700 - 03: Distributed Deployment
- **CIS Mapping**:
  - CIS Control: 6.5 (Geographic Distribution)
- **CSA CCM Mapping**:
  - CSA CCM: GRM-01 (Governance and Risk Management)
- **Implementation**:
  - Use cloud provider's multi-region deployment capabilities.
  - Distribute data replicas in geographically distant regions.
  - With the exception if global resources, no resource must be deployed outside of EastUS, unless required.

---

## Firewall and Access Control Standards

### Standard 700 - 03: Traffic Filtering

- **Description**: Implement stateful and stateless packet filtering to control traffic.
- **Policy Mapping**:
  - Policy 700 - 05: Default Policy
- **CIS Mapping**:
  - CIS Control: 9.2 (Limitation and Control of Network Ports)
- **CSA CCM Mapping**:
  - CSA CCM: NET-01 (Network Architecture)
- **Implementation**:
  - Default deny-all inbound and outbound rules for PaaS and IaaS infrastructure.
  - Allow specific traffic based on the source, destination, and port requirements.

---

### Standard 700 - 04: Network Activity Logging

- **Description**: Capture logs for all network-related activities.
- **Policy Mapping**:
  - Policy 700 - 07: Logging
- **CIS Mapping**:
  - CIS Control: 6.2 (Incident Event Logging)
- **CSA CCM Mapping**:
  - CSA CCM: LOG-05 (Centralized Logging)
- **Implementation**:
  - Use cloud-native or third-party logging solutions.
  - Store logs in a centralized and secure location.

---

## Subnet Access Control Standards

### Standard 700 - 05: Granular Subnet Controls

- **Description**: Ensure fine-grained access controls at the subnet level.
- **Policy Mapping**:
  - Policy 700 - 08: Design
- **CIS Mapping**:
  - CIS Control: 14.8 (Wireless Device Access Control)
- **CSA CCM Mapping**:
  - CSA CCM: NET-03 (Network Segmentation)
- **Implementation**:
  - Differentiate subnets for production, staging, and development environments.
  - Implement strict ACLs for production subnets.

---

## Private Connectivity and Secure Data Transfer Standards

### Standard 700 - 06: End-to-End Encryption

- **Description**: Mandate encryption for data in transit between any two points.
- **Policy Mapping**:
  - Policy 700 - 12: Encryption
- **CIS Mapping**:
  - CIS Control: 13.1 (Protect Data in Transit)
- **CSA CCM Mapping**:
  - CSA CCM: EKM-01 (Encryption and Key Management)
- **Implementation**:
  - Use TLS 1.2 or higher for all connections.
  - Encrypt VPN tunnels with strong cryptographic algorithms.

---

### Standard 700 - 07: Private Connection Monitoring

- **Description**: Continuously monitor private connections for disruptions or unauthorized activities.
- **Policy Mapping**:
  - Policy 700 - 14: Monitoring
- **CIS Mapping**:
  - CIS Control: 8.3 (Malware Defenses)
- **CSA CCM Mapping**:
  - CSA CCM: SEF-01 (System and Network Event Monitoring)
- **Implementation**:
  - Set up monitoring tools with real-time alerting capabilities.
  - Regularly audit connection logs.

---

## General Best Practices

### Standard 700 - 08: Patch Management

- **Description**: Ensure that all cloud assets are patched regularly.
- **Policy Mapping**:
  - General Best Practices
- **CIS Mapping**:
  - CIS Control: 2.2 (Software Inventory and Patching)
- **CSA CCM Mapping**:
  - CSA CCM: CCS-05 (Change Management and Control)
- **Implementation**:
  - Automate patching using cloud-native or third-party tools.
  - Implement a rollback strategy in case of update failures.

---

### Standard 700 - 09: Regular Audits (Under Review)

- **Description**: Perform security audits at regular intervals to check compliance with these standards.
- **Policy Mapping**:
  - Policy 700 - 05: Review and Update
- **CIS Mapping**:
  - CIS Control: 20.3 (Penetration Tests and Red Team Exercises)
- **CSA CCM Mapping**:
  - CSA CCM: APT-01 (Application and Interface Security)
- **Implementation**:
  - Engage third-party security experts for unbiased reviews.
  - Remediate identified gaps within a stipulated time frame.

### Standard 700 - 10: IP Restrictions (Under Review)

- **Description**: Restrict network access by removing or disallowing public IP addresses when possible. (Under Review)
- **Policy Mapping**:
  - Policy 700 - 05: Default Policy
- **CIS Mapping**:
  - CIS Control: 20.3 (Penetration Tests and Red Team Exercises)
- **CSA CCM Mapping**:
  - CSA CCM: APT-01 (Application and Interface Security)
- **Implementation**:
  - Implement Azure policies and SCPs to prevent the creation of public IP addresses.
  - Prevent public IP addresses from being associated with network resources via Azure policies and SCPs.

### Standard 700 - 11: Cloud Storage Firewall (Under Review)

- **Description**: All cloud storage accounts must be associated with a firewall, restricting inbound access. (Under Review)
- **Policy Mapping**:
  - Policy 700 - 03: Distributed Deployment
- **CIS Mapping**:
  - CIS Control: 20.3 (Penetration Tests and Red Team Exercises)
- **CSA CCM Mapping**:
  - CSA CCM: APT-01 (Application and Interface Security)
- **Implementation**:
  - Implement Azure policies and SCPs to prevent the creation of public IP addresses.
  - Prevent public IP addresses from being associated with network resources via Azure policies and SCPs.