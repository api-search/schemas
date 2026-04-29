---
description: CashFlowSummary schema from ARGUS Enterprise API
layout: schema
name: CashFlowSummary
properties_list:
- description: Total revenue over the analysis period
  name: totalRevenue
  type: number
- description: Total expenses over the analysis period
  name: totalExpenses
  type: number
- description: Total net operating income
  name: totalNOI
  type: number
- description: Total capital expenditures
  name: totalCapEx
  type: number
- description: Average occupancy rate (percentage)
  name: averageOccupancy
  type: number
- description: Internal rate of return (percentage)
  name: irr
  type: number
- description: Net present value
  name: npv
  type: number
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-cash-flow-summary-schema.json
slug: argus-enterprise-cash-flow-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-cash-flow-summary-schema.json\",\n  \"title\": \"CashFlowSummary\",\n  \"description\": \"CashFlowSummary schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalRevenue\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total revenue over the analysis period\"\n    },\n    \"totalExpenses\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total expenses over the analysis period\"\n    },\n    \"totalNOI\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total net operating income\"\n    },\n    \"totalCapEx\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total capital expenditures\"\n \
  \   },\n    \"averageOccupancy\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Average occupancy rate (percentage)\"\n    },\n    \"irr\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Internal rate of return (percentage)\"\n    },\n    \"npv\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Net present value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-cash-flow-summary-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: CashFlowSummary
---
