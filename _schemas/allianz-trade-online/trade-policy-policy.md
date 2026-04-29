---
description: A trade credit insurance policy from Allianz Trade
layout: schema
name: Policy
properties_list:
- description: Unique identifier for the policy
  name: policyId
  type: string
- description: Official Allianz Trade policy number
  name: policyNumber
  type: string
- description: Legal name of the policy holder
  name: policyHolderName
  type: string
- description: Type of trade credit insurance policy
  name: policyType
  type: string
- description: Current status of the policy
  name: policyStatus
  type: string
- description: ISO 4217 policy currency code
  name: currency
  type: string
- description: Maximum total coverage amount under the policy
  name: maxCoverageAmount
  type: number
- description: Percentage of loss covered by the policy
  name: coveragePercentage
  type: integer
- description: Policy start date
  name: startDate
  type: string
- description: Policy end date
  name: endDate
  type: string
- description: ISO 3166-1 alpha-2 country code for the policy
  name: country
  type: string
- description: Timestamp when the policy was created
  name: createdAt
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-policy-policy-schema.json
slug: trade-policy-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-policy-policy-schema.json\",\n  \"title\": \"Policy\",\n  \"type\": \"object\",\n  \"description\": \"A trade credit insurance policy from Allianz Trade\",\n  \"properties\": {\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the policy\"\n    },\n    \"policyNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Official Allianz Trade policy number\"\n    },\n    \"policyHolderName\": {\n      \"type\": \"string\",\n      \"description\": \"Legal name of the policy holder\"\n    },\n    \"policyType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of trade credit insurance policy\",\n      \"enum\": [\n        \"trade_credit\",\n        \"surety\",\n        \"ecommerce_b2b\"\n      ]\n    },\n    \"policyStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current\
  \ status of the policy\",\n      \"enum\": [\n        \"active\",\n        \"suspended\",\n        \"expired\",\n        \"cancelled\"\n      ]\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 policy currency code\"\n    },\n    \"maxCoverageAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Maximum total coverage amount under the policy\"\n    },\n    \"coveragePercentage\": {\n      \"type\": \"integer\",\n      \"description\": \"Percentage of loss covered by the policy\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy start date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy end date\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code for\
  \ the policy\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the policy was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-policy-policy-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: Policy
---
