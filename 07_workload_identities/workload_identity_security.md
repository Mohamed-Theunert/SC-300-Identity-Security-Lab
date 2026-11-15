# Workload Identity Security

## Objective

Understand and secure non-human identities.

## Examples

- Service principals
- Managed identities
- Application registrations
- Automation identities

## Risks

- Excessive API permissions
- Long-lived client secrets
- Unused applications
- Privileged service principals
- Secrets stored in scripts
- Unreviewed application consent

## Lab Checklist

- Review application registrations
- Review service principals
- Identify high-privilege API permissions
- Review credential expiry
- Prefer managed identities where appropriate
- Remove unused credentials
- Document application owners

## Investigation Questions

- Which identity performed the action?
- Which permissions does it have?
- Which credentials are configured?
- When were credentials last rotated?
- Is admin consent present?
- Does the application still have a valid business purpose?
