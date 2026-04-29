---
description: CashFlowProjection schema from ARGUS Enterprise API
layout: schema
name: CashFlowProjection
properties_list:
- description: Associated property identifier
  name: propertyId
  type: string
- description: Projection start date
  name: startDate
  type: string
- description: Projection end date
  name: endDate
  type: string
- description: Cash flow reporting frequency
  name: frequency
  type: string
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Individual cash flow periods
  name: periods
  type: array
- description: ''
  name: summary
  type: object
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-cash-flow-projection-schema.json
slug: argus-enterprise-cash-flow-projection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-cash-flow-projection-schema.json\",\n  \"title\": \"CashFlowProjection\",\n  \"description\": \"CashFlowProjection schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"propertyId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Associated property identifier\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Projection start date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Projection end date\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Monthly\",\n        \"Quarterly\",\n        \"Annual\"\n      ],\n      \"description\": \"Cash flow\
  \ reporting frequency\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\"\n    },\n    \"periods\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CashFlowPeriod\"\n      },\n      \"description\": \"Individual cash flow periods\"\n    },\n    \"summary\": {\n      \"$ref\": \"#/components/schemas/CashFlowSummary\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-cash-flow-projection-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: CashFlowProjection
---
