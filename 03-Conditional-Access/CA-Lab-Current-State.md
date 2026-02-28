# Conditional Access – Current Lab State

## 🎯 Objective

Document the currently implemented Conditional Access baseline policies in the lab environment.

---

# 1️⃣ CA - Require MFA for All Users

## Scope

Users:
- All users
- (Break-glass account excluded if configured)

Cloud apps:
- All cloud apps

Grant control:
- Require Multi-Factor Authentication (MFA)

## Security Impact

- Eliminates password-only authentication
- Reduces credential theft risk
- Establishes Zero Trust baseline

## Risk Mitigated

- Password spray attacks
- Stolen credentials reuse
- Phishing without MFA bypass

---

# 2️⃣ CA - Block Non-Germany Logins

## Scope

Users:
- All users (unless excluded)

Condition:
- Locations → Block access outside Germany

Grant control:
- Block access

## Security Impact

- Reduces attack surface from foreign IP ranges
- Limits brute force attempts from high-risk regions

## Considerations

- Requires correct Named Location configuration
- VPN usage may bypass country-based logic
- Not recommended as sole protection mechanism in production
