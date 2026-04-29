---
description: LeaseInput schema from ARGUS Enterprise API
layout: schema
name: LeaseInput
properties_list:
- description: ''
  name: tenantId
  type: string
- description: ''
  name: unitNumber
  type: string
- description: ''
  name: leaseType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: leasedArea
  type: number
- description: ''
  name: baseRent
  type: number
- description: ''
  name: rentFrequency
  type: string
- description: ''
  name: escalationRate
  type: number
- description: ''
  name: escalationType
  type: string
- description: ''
  name: securityDeposit
  type: number
- description: ''
  name: tenantImprovementAllowance
  type: number
- description: ''
  name: currency
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-lease-input-schema.json
slug: argus-enterprise-lease-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-lease-input-schema.json\",\n  \"title\": \"LeaseInput\",\n  \"description\": \"LeaseInput schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tenantId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"unitNumber\": {\n      \"type\": \"string\"\n    },\n    \"leaseType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Gross\",\n        \"Net\",\n        \"DoubleNet\",\n        \"TripleNet\",\n        \"ModifiedGross\",\n        \"PercentageRent\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Expired\",\n        \"Pending\"\n      ],\n      \"default\": \"Active\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"leasedArea\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"baseRent\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"rentFrequency\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Monthly\",\n        \"Quarterly\",\n        \"Annual\"\n      ],\n      \"default\": \"Monthly\"\n    },\n    \"escalationRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"escalationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Fixed\",\n        \"CPI\",\n        \"MarketReset\",\n        \"StepUp\"\n      ]\n    },\n    \"securityDeposit\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"tenantImprovementAllowance\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n     \
  \ \"default\": \"USD\"\n    }\n  },\n  \"required\": [\n    \"tenantId\",\n    \"leaseType\",\n    \"startDate\",\n    \"endDate\",\n    \"baseRent\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-lease-input-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: LeaseInput
---
