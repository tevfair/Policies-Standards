| Version | Author         | Description                       | Date      |
|---------|----------------|-----------------------------------|-----------|
| 1.0     | Tevin Fair  | Initial publication |08/11/2024 |

## Table of Contents

- [Development and DevOps](#development-and-devops)
- [Infrastructure as Code (IaC) Security Checks](#infrastructure-as-code)
- [Continuous Integration/Continuous Deployment (CI/CD) Security Checks](#cicd-security-checks)
---
## Development and DevOps

### Policy 900 - 01: Code Repository Security

- **Description**: Ensure secure and controlled access to all source code repositories.
- **Associated Guideline**:
  - Repositories should be private and access-controlled with enabled logging for every access or change.
  - Conduct regular audits of user access to repositories.
  - Mandate two-factor authentication (2FA) for accessing code repositories.

### Policy 900 - 02: Secure Software Development Life Cycle (SDLC)

- **Description**: Ensure the integration of security reviews and assessments at all stages of the SDLC.
- **Associated Guideline**:
  - Incorporate security reviews and vulnerability assessments in all SDLC stages.
  - Provide periodic training on secure coding practices to developers.

---

<a name="infrastructure-as-code"></a>

## Infrastructure as Code (IaC) Security Checks

### Policy 900 - 03: Version Control

- **Description**: Maintain and control versions of all Infrastructure as Code configurations.
- **Associated Guideline**:
  - Store all IaC configurations in version-controlled repositories.
  - Retain historical versions for a duration mandated by compliance requirements.

### Policy 900 - 04: Configuration Validation

- **Description**: Authenticate and verify any IaC changes for security misconfigurations before implementation.
- **Associated Guideline**:
  - Validate configurations for security misconfigurations before applying IaC changes.
  - Use automated tools for static analysis on IaC templates to detect vulnerabilities.

### Policy 900 - 05: Least Privilege Principle

- **Description**: IaC configurations should operate under the least privilege principle.
- **Associated Guideline**:
  - Only grant necessary permissions required for operations in IaC configurations.

### Policy 900 - 06: Secrets Management

- **Description**: Prohibit the hardcoding of sensitive data into IaC scripts and ensure its secured storage.
- **Associated Guideline**:
  - Avoid hardcoding sensitive details like API keys or passwords in IaC scripts.
  - Utilize secret managers or encrypted storage solutions.

---

<a name="cicd-security-checks"></a>

## Continuous Integration/Continuous Deployment (CI/CD) Security Checks

### Policy 900 - 07: Automated Security Testing

- **Description**: Integrate automated security tests in CI/CD pipelines to scan for potential vulnerabilities.
- **Associated Guideline**:
  - Embed automated security testing tools in CI/CD pipelines.
  - Regularly scan codebase and dependencies for vulnerabilities.

### Policy 900 - 08: Dependency Management

- **Description**: Ensure the security and updated status of all dependencies.
- **Associated Guideline**:
  - Utilize automated tools to scan dependencies for recognized vulnerabilities.
  - Update or replace outdated or vulnerable dependencies promptly.

### Policy 900 - 09: Immutable Infrastructure

- **Description**: Aim for immutable infrastructure in CI/CD deployments.
- **Associated Guideline**:
  - Target creating an immutable infrastructure in CI/CD deployments where once deployed, resources aren't modified but replaced by new versions.

### Policy 900 - 10: Access Control

- **Description**: Restrict access to CI/CD tools and maintain comprehensive activity logs.
- **Associated Guideline**:
  - Limit CI/CD tool access to authorized personnel only.
  - Uphold comprehensive audit logs for all CI/CD activities.

### Policy 900 - 11: Artifact Management

- **Description**: Securely store build artifacts in access-controlled repositories and ensure their integrity.
- **Associated Guideline**:
  - Store all build artifacts in secure, access-controlled repositories.
  - Authenticate and verify artifact integrity prior to deployment.

### Policy 900 - 12: Environment Isolation

- **Description**: Maintain isolation between production and non-production environments.
- **Associated Guideline**:
  - Ensure clear separation between production and other environments.
  - Avoid direct deployments to production without transitioning through staging/testing phases.
