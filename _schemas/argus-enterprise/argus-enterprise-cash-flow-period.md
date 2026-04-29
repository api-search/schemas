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
source_filename: argus-enterprise-cash-flow-period-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-cash-flow-period-schema.json\",\n  \"title\": \"CashFlowPeriod\",\n  \"description\": \"CashFlowPeriod schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"periodStart\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Period start date\"\n    },\n    \"periodEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Period end date\"\n    },\n    \"grossPotentialRent\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Gross potential rental income\"\n    },\n    \"vacancyLoss\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Vacancy and credit loss\"\n    },\n    \"effectiveGrossIncome\": {\n      \"\
  type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Effective gross income after vacancy\"\n    },\n    \"otherIncome\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Other income (parking, storage, etc.)\"\n    },\n    \"totalRevenue\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total revenue\"\n    },\n    \"operatingExpenses\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total operating expenses\"\n    },\n    \"netOperatingIncome\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Net operating income (NOI)\"\n    },\n    \"capitalExpenditures\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Capital expenditure costs\"\n    },\n    \"tenantImprovements\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Tenant\
  \ improvement costs\"\n    },\n    \"leasingCommissions\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Leasing commission costs\"\n    },\n    \"debtService\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Debt service payments\"\n    },\n    \"cashFlowBeforeDebt\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Cash flow before debt service\"\n    },\n    \"cashFlowAfterDebt\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Cash flow after debt service\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-cash-flow-period-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: CashFlowPeriod
---
