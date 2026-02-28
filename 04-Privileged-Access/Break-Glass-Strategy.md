# Break-Glass Account Strategy

## 🎯 Objective

Provide emergency access in case Conditional Access, MFA or identity infrastructure fails.

---

## Account Configuration

Account name:
- emergency-admin

Role:
- Global Administrator

Authentication:
- Strong password (20+ characters)
- No MFA registered

---

## Conditional Access Exclusion

The account is excluded from:
- All Conditional Access policies
- All risk-based access policies

---

## Security Considerations

- Password stored securely
- Account not used for daily administration
- Sign-in activity monitored
- Alert triggered on login

---

## Risk

If compromised, attacker gains full tenant access.

Therefore:
- Monitor aggressively
- Never use for normal operations
