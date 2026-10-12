# IAM Access Review Audit Findings

Prepared by: Andrea Hudson (GRC Analyst)  
Date: 2026-10-12

## Scope
Quarterly access review of privileged and high-risk roles across finance, HR, IT, and security.

## Summary of findings
- 3 users with excess or obsolete access were identified
- 1 dormant account was removed from the role-based access list
- 2 privileged access users required documented justification and approval

## Key findings
1. Excess access after role changes
   - User U001 removed from Finance admin access after manager confirmation that role no longer existed.
   - User U003 removed from Windows admin after separation from contractor status.

2. Dormant access
   - User U005 had no access activity for more than 180 days and no documented business need.
   - Access was removed after review and ticket closure.

3. Privileged access governance
   - U007 retained privileged access under formal business justification.
   - Access reviewed with approval documentation and periodic recertification requirement.

## Risk rating
- Medium overall risk.
- High risk if left unreviewed: privilege creep, orphan accounts, and access drift.

## Recommended next steps
- Implement automated quarterly recertification for all privileged roles.
- Remove dormant accounts after 90 days of inactivity unless approved.
- Require manager attestation for any privileged access.
- Track exceptions and review them monthly.

## Final recommendation
Approve the access review with remediation actions implemented and a recurring quarterly cycle.

## KPI examples
- 100% of privileged users reviewed
- 3 stale accounts removed
- 2 privileged access exceptions documented and approved
