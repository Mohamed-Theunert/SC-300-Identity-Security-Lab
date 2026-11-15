# Emergency Access (Break-Glass) Strategy

## Objective

Provide resilient emergency administrative access when normal authentication, Conditional Access, federation, or identity services are unavailable.

## Account Design

Recommended baseline:

- Maintain at least **two** emergency access accounts for redundancy.
- Use **cloud-only** accounts in the tenant's `.onmicrosoft.com` domain.
- Assign the **Global Administrator** role as permanently active for the emergency accounts.
- Do not use the accounts for normal administrative work.

Example lab names:

- emergency-admin-01
- emergency-admin-02

## Authentication

Use a phishing-resistant authentication method that is independent from the normal administrator authentication path.

Preferred options:

- Passkey / FIDO2 security key
- Certificate-Based Authentication (CBA), where PKI is already available

Avoid designing emergency access around a single dependency that could fail during the same outage.

## Conditional Access

Emergency access accounts should be excluded from Conditional Access policies that could block or restrict emergency sign-in.

The exclusion is intentional and must be compensated by:

- Strong phishing-resistant authentication
- Strict monitoring
- Restricted use
- Secure credential storage
- Regular validation

## Security Controls

- Monitor every sign-in and audit event for the emergency accounts.
- Alert on any use of the accounts.
- Store credentials or security keys in secure, separate locations.
- Use a designated secure administrative workstation where possible.
- Ensure credentials and authentication devices do not expire unexpectedly.
- Review authorized users regularly.
- Validate emergency access at least every 90 days.

## Risk

Emergency access accounts have extremely high privilege.

If one is compromised, an attacker could obtain tenant-wide administrative control.

Therefore:

- Never use emergency accounts for day-to-day administration.
- Investigate every sign-in.
- Keep the emergency access process documented and tested.
