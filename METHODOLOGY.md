# GRC Risk Methodology and Portfolio Scoring Framework

This document defines the methodology used in the portfolio and explains how risk is evaluated across the vendor risk, IAM review, and vulnerability workstreams.

## 1. Risk Assessment Approach
The portfolio uses a practical GRC approach that is simple, transparent, and aligned to real-world security operations.

### Step 1: Establish context
Before scoring risk, I determine:
- the type of asset or vendor involved
- the sensitivity of data involved (for example, PHI, PII, internal-only data)
- the business criticality of the service
- exposure to users, the internet, or third parties

### Step 2: Gather evidence
Evidence may include:
- questionnaires
- policy documents
- attestations and audit reports
- IT asset information
- access review results
- vulnerability scan outputs
- system or role descriptions

### Step 3: Identify gaps
I assess whether the control or process is:
- implemented
- partially implemented
- not implemented

This is documented clearly so a reviewer can understand both the positive controls and the areas needing remediation.

## 2. Risk Scoring Model
For the vendor risk example, I use a simple likelihood × impact model.

- likelihood: 1 to 5
- impact: 1 to 5
- score: likelihood × impact

Example:
- likelihood = 4
- impact = 5
- score = 20

### Typical interpretation
- 1–6: Low risk
- 7–14: Medium risk
- 15–25: High / critical risk

This model is intentionally simple and useful for interviews, review discussions, and practical governance tracking.

## 3. Control and Framework Mapping
Where applicable, I map findings to recognized control frameworks, including:
- NIST Cybersecurity Framework (CSF)
- NIST SP 800-53
- HIPAA Security Rule

This helps connect the assessment to accepted control language and helps business stakeholders understand which requirements are not being met.

## 4. Access Review Methodology
The IAM access review focuses on:
- valid business need for access
- role alignment and entitlement review
- stale or inactive accounts
- privileged access justification
- separation of duties and access drift

A user is considered a risk if their access:
- is no longer required
- is assigned to a role they no longer hold
- is dormant or unused for an extended period
- is privileged without documented business justification

## 5. Vulnerability Prioritization Methodology
The vulnerability management example uses a mix of:
- CVSS v3 score
- exposure (internet-facing vs. internal)
- asset criticality
- remediation age or SLA timeline

This is important because not every high CVSS issue is equally urgent if it is not exposed or not business-critical.

## 6. Recommendation Logic
The portfolio uses practical risk recommendation logic:
- approve when controls are adequate and residual risk is acceptable
- approve with conditions when evidence is mostly good but a few gaps remain
- escalate or reject when risk exceeds tolerance or when business justification is weak

## 7. Assumptions and Limitations
This portfolio uses synthetic data for demonstration purposes. In a real organization, additional information would be required such as:
- actual contracts and legal terms
- complete policy and architecture documentation
- system inventory and asset owners
- current control testing results
- audit and compliance evidence

## 8. Summary
This portfolio reflects a realistic GRC mindset:
- understand the business context
- validate evidence
- prioritize based on impact and exposure
- define actionable remediation
- communicate decisions clearly to leadership

The result is a risk story that is both operational and executive-friendly.
