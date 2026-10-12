# Presentation slides and speaker notes (healthcare-vendor-risk-presentation)

## Slide 1 — Title: Vendor Risk Assessment — Example Health Tech
Notes: "Hello — I’m Andrea Hudson. Today I’ll walk through a vendor risk assessment for a patient-portal provider and show the remediation plan and KPIs. Bottom line: conditional approval pending a penetration test and clarified incident response RTOs."

## Slide 2 — Agenda
- Scope
- Evidence
- Control mapping
- Risk scoring
- Remediation
- KPIs
- Decision

Notes: "I’ll follow this flow so the assessment is easy to understand."

## Slide 3 — Scope & Business Impact
- Vendor: Example Health Tech
- Service: Patient portal and patient messaging
- Data handled: PHI + PII
- Criticality: High

Notes: "We classified this vendor as High because it handles PHI. That drives stronger assurance requirements and shorter remediation windows."

## Slide 4 — Intake Summary
Visual: table from Vendors sheet (vendor, service, criticality)

Notes: "This intake record captures the scope, business owner, and classification. It is the starting point for the review."

## Slide 5 — Questionnaire Highlights
- Positive: encryption, MFA, scans, IR plan
- Negative: no annual pen-test, no SOC 2 attestation

Notes: "Key controls are present, but the lack of independent validation is the main gap."

## Slide 6 — Control Mapping
Visual: map missing items to NIST/HIPAA (e.g., pentest -> NIST CA-2)

Notes: "Mapping helps legal and engineering convert gaps into contractual requirements."

## Slide 7 — Risk Register (top risks)
Visual: R001 (score 20) and R002 (score 12)

Notes: "R001 is the highest-priority item; remediation is contractual and operational."

## Slide 8 — Remediation & Contractual Asks
- Require pen-test within 90 days and remediation within 30 days for critical findings
- Define IR RTOs and run tabletop within 60 days
- Document backup encryption

Notes: "These are tracked in the risk register and via tickets."

## Slide 9 — KPIs & Monitoring Plan
- Open high risks: 1
- % critical remediated in SLA: target 95%
- Avg time to remediate: tracked monthly

Notes: "Report to security steering committee monthly."

## Slide 10 — Decision & Next Steps
- Recommendation: Conditional approval
- Conditions: pen-test evidence, IR RTOs, remediation plan
- Review date: 90 days

Notes: "Conditional approval with a clear path to full approval once evidence is provided."
