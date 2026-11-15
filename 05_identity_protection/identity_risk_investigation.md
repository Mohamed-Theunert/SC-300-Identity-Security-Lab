# Identity Risk Investigation

## Objective

Practice investigating risky users and risky sign-ins.

## Concepts

- User risk
- Sign-in risk
- Risk detections
- Risk remediation
- Risk-based Conditional Access

## Investigation Workflow

```text
Risk detected
    ↓
Identify user
    ↓
Review sign-in
    ↓
Review IP / location / device
    ↓
Check MFA result
    ↓
Review surrounding sign-ins
    ↓
Check related alerts
    ↓
Determine benign vs suspicious
    ↓
Remediate / dismiss / escalate
```

## Evidence to Review

- Sign-in time
- IP address
- Location
- Device
- Application
- Authentication method
- MFA result
- Previous user activity
- Related Defender or Sentinel alerts

## False-Positive Considerations

- Corporate VPN
- Mobile networks
- Cloud proxies
- Travel
- Shared egress IPs

## Escalation

Escalate when:
- Privileged user affected
- Token theft suspected
- MFA anomalies observed
- Multiple risky sign-ins occur
- Suspicious activity follows authentication
