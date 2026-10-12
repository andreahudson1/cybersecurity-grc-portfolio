# healthcare-vendor-risk-workbook instructions

This file describes how to create the Excel workbook (`healthcare-vendor-risk-workflow.xlsx`) from the CSVs included in this repo.

## Sheets to create
- Vendors (table name: `Vendors`) — import `vendor-intake.csv`
- Questionnaire (table name: `Questionnaire`) — import `security-questionnaire.csv`
- ControlMap (table name: `ControlMap`) — import `control-mapping.csv`
- RiskRegister (table name: `RiskRegister`) — import `risk-register.csv`
- Dashboard — create KPIs and pivot tables
- Evidence — optional evidence index

## Key formulas
- Risk Register Score: `=[@[likelihood(1-5)]]*[@[impact(1-5)]]`
- Residual risk: `=IFS([@score]>=15,"High",[@score]>=7,"Medium",TRUE,"Low")`

## Conditional formatting
Apply to the Score column:
- `>=15` → Red fill
- `7–14` → Yellow fill
- `<=6` → Green fill

## Dashboard formulas
- OpenHighCount: `=COUNTIFS(RiskRegister[status],"Open",RiskRegister[score],">=15")`
- AvgDaysToClose: `=IFERROR(AVERAGEIFS(RiskRegister[days_to_close],RiskRegister[status],"Closed"),"n/a")`

Use the workbook to track owner assignments, tickets, SLA days, and evidence links. Convert data ranges into tables for robust formulas and pivots.
