# Final Assessment: Example Health Tech (Vendor V001)

Prepared by: Andrea Hudson (GRC Analyst) — synthetic example  
Date: 2026-10-12

## Executive summary
- Service: Patient portal (handles PHI).
- Overall recommendation: Approve with conditions.
- Rationale: Vendor demonstrates strong encryption and MFA controls, incident response plan exists, and regular vulnerability scanning is in place. However, the absence of a formal annual penetration test and incomplete IR RTO definitions are notable gaps for a high-criticality PHI processing vendor. Mitigations are required prior to full approval.

## Top findings (prioritized)
1) Missing annual penetration test (Risk R001) — Score 20 (High/Critical). Action: vendor to perform pen-test within 90 days and provide remediation proof. Contractual requirement and evidence required before go-live for any new integration.
2) IR plan lacks explicit RTO definitions (Risk R002) — Score 12 (Medium). Action: vendor to define RTOs and run a tabletop in 60 days; share summary report.
3) Other controls (encryption at rest/transit, MFA for admin, regular scans) are implemented and validated.

## Recommended contractual clauses & controls
- Penetration testing clause: annual pen-test with written remediation plan; critical findings remediated within 30 days.
- Right-to-audit: vendor to provide SOC 2 or equivalent within 12 months.
- Data handling addendum: require explicit mapping of PHI flows and encryption of backups.
- Incident notification SLA: notify within 24 hours of confirmed breach with delivery of IR timeline.

## Monitoring and acceptance criteria
- Acceptance (conditions met) when vendor provides: (a) completed pen-test report with closure evidence, (b) documented RTOs and tabletop summary, (c) updated backup encryption documentation.
- Ongoing monitoring: quarterly vulnerability scan reports and semi-annual control attestations.

## KPI / metrics to track (initial baseline)
- Number of open high/critical vendor risks: 1 (R001).
- Time to remediation (target): critical findings <30 days, high findings <60 days.
- Evidence frequency: quarterly scans + annual attestation.

## Decision
- Conditional Approval: allow integration for non-critical patient workflows only after immediate compensating controls and issue tracking; full approval upon evidence of pen-test and remediation.

Appendix: risk register excerpt, questionnaire evidence links, control mapping summary.
