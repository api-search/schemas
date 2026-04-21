---
description: CashFlowPeriod schema from ARGUS Enterprise API
layout: schema
name: CashFlowPeriod
properties_list:
- description: Period start date
  name: periodStart
  type: string
- description: Period end date
  name: periodEnd
  type: string
- description: Gross potential rental income
  name: grossPotentialRent
  type: number
- description: Vacancy and credit loss
  name: vacancyLoss
  type: number
- description: Effective gross income after vacancy
  name: effectiveGrossIncome
  type: number
- description: Other income (parking, storage, etc.)
  name: otherIncome
  type: number
- description: Total revenue
  name: totalRevenue
  type: number
- description: Total operating expenses
  name: operatingExpenses
  type: number
- description: Net operating income (NOI)
  name: netOperatingIncome
  type: number
- description: Capital expenditure costs
  name: capitalExpenditures
  type: number
- description: Tenant improvement costs
  name: tenantImprovements
  type: number
- description: Leasing commission costs
  name: leasingCommissions
  type: number
- description: Debt service payments
  name: debtService
  type: number
- description: Cash flow before debt service
  name: cashFlowBeforeDebt
  type: number
- description: Cash flow after debt service
  name: cashFlowAfterDebt
  type: number
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-cash-flow-period-schema.json
slug: argus-enterprise-cash-flow-period
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: CashFlowPeriod
---
