# Identity Monitoring & KQL

## Objective

Use Entra logs for identity-security investigations and control validation.

## Primary Tables

### SigninLogs
Useful for:
- Successful and failed sign-ins
- Source IPs
- Applications
- Authentication results
- Conditional Access outcomes
- Location and device context

### AuditLogs
Useful for:
- Role changes
- User/group changes
- Application changes
- Consent events
- Administrative activity

## Learning Workflow

1. Start broad.
2. Inspect actual fields.
3. Establish normal behavior.
4. Filter suspicious patterns.
5. Correlate with surrounding activity.
6. Convert stable hunting logic into a detection only after tuning.

## Included Queries

- Entra-Signin-Baseline.kql
- Failed-Signins.kql
- Privileged-Role-Changes.kql
