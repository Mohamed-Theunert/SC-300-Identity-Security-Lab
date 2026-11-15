# Privileged Identity Management Lab

## Objective

Reduce standing administrative privilege by using just-in-time elevation.

## Concepts

- Eligible assignment
- Active assignment
- Activation
- Approval
- MFA requirement
- Activation duration
- Access review
- Audit history

## Lab Scenario

Create a privileged role assignment as eligible instead of permanently active.

Validate:

1. User cannot perform privileged action before activation.
2. User activates the role.
3. Required controls are enforced.
4. Privileged action becomes available.
5. Role expires after the configured duration.
6. Activation is visible in audit history.

## Security Benefit

PIM reduces the time window in which privileged permissions are continuously available.

## Investigation Questions

- Who activated the role?
- Which role?
- When?
- From which account/device?
- Was approval required?
- What actions occurred during the activation window?
