# Authentication Methods Lab

## Objective

Understand how authentication method choice affects identity security.

## Topics

- Password authentication
- Microsoft Authenticator
- Passkeys / FIDO2 security keys
- Certificate-Based Authentication
- Authentication strengths
- Phishing-resistant authentication

## Lab Goals

1. Review enabled authentication methods.
2. Identify which methods are phishing resistant.
3. Compare normal MFA with phishing-resistant MFA.
4. Document which users or roles should require stronger authentication.
5. Review recovery and registration considerations.

## Security Considerations

Authentication strength should match account risk.

Examples:

- Standard user → strong MFA
- Privileged administrator → phishing-resistant MFA preferred
- Emergency access → independent, resilient authentication path

## Validation

Confirm:
- Registration works as expected
- Conditional Access recognizes the authentication method
- Recovery paths are documented
- Privileged accounts do not rely on weak fallback methods
