# Conditional Access Design Checklist

## Objective

Design Conditional Access policies without creating accidental lockouts or unnecessary policy overlap.

## Before Creating a Policy

Document:

- Target users/groups
- Exclusions
- Target resources
- Conditions
- Grant controls
- Session controls
- Report-only testing plan

## Recommended Workflow

1. Define the threat or risk being addressed.
2. Create a small pilot group.
3. Configure the policy in report-only mode where appropriate.
4. Review sign-in impact.
5. Validate exclusions.
6. Move to enforced state.
7. Monitor failures and false positives.

## Important Exclusions

Emergency access accounts require deliberate exclusion from policies that could block emergency sign-in.

## Common Mistakes

- Targeting all users without emergency exclusions
- Creating overlapping policies without documenting interaction
- Blocking locations without accounting for VPN/proxy traffic
- Enforcing before reviewing report-only results
- Relying on one control as the only protection
