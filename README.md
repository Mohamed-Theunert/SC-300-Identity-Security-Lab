# SC-300 Identity Security Lab

Hands-on learning repository for Microsoft Entra ID identity security, access control, governance, privileged access, authentication, and monitoring.

The repository is structured as a practical lab environment rather than a collection of exam notes. Each section is intended to document concepts, lab goals, validation steps, security considerations, and lessons learned.

## Lab Areas

```text
.
├── 01-Identity-Fundamentals/
├── 02-Authentication-Methods/
├── 03-Conditional-Access/
├── 04-Privileged-Access/
├── 05-Identity-Protection/
├── 06-Identity-Governance/
├── 07-Workload-Identities/
└── 08-Monitoring-KQL/
```

## Focus

- Microsoft Entra ID
- Identity & Access Management
- Authentication methods
- Passkeys / FIDO2
- Conditional Access
- Emergency access
- Privileged Identity Management
- Identity Protection
- Access Reviews
- Entitlement Management
- Workload identities
- Identity monitoring with KQL
- Security-focused lab documentation

## Lab Method

Each lab follows the same workflow:

```text
Understand the control
        ↓
Define the security goal
        ↓
Configure in the lab
        ↓
Validate expected behavior
        ↓
Document edge cases
        ↓
Review security impact
        ↓
Record lessons learned
```

## Current Sections

### 01 — Identity Fundamentals
Tenant, users, groups, administrative roles, and identity-security concepts.

### 02 — Authentication Methods
Authentication methods, phishing resistance, passkeys / FIDO2, and authentication-strength concepts.

### 03 — Conditional Access
Conditional Access baseline design, exclusions, locations, and policy validation.

### 04 — Privileged Access
Emergency access strategy, privileged administration, and PIM concepts.

### 05 — Identity Protection
User risk, sign-in risk, risk-based Conditional Access, and investigation workflow.

### 06 — Identity Governance
Access Reviews, entitlement lifecycle, and periodic access validation.

### 07 — Workload Identities
Service principals, managed identities, application permissions, and non-human identity security.

### 08 — Monitoring & KQL
Entra sign-in and audit monitoring with KQL for investigations and security validation.

## Security Principle

Identity controls should be designed so that a single misconfiguration does not create either a lockout condition or a major privilege-escalation path.

## Notes

- This is a lab and learning repository.
- Configuration examples must be validated before production use.
- All identities and examples are fictional.
- No organization-specific or sensitive information is stored here.
