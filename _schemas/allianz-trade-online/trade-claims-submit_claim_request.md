---
description: Request body for submitting an insurance claim
layout: schema
name: SubmitClaimRequest
properties_list:
- description: Trade credit insurance policy identifier
  name: policyId
  type: string
- description: Name of the defaulting debtor
  name: debtorName
  type: string
- description: Allianz Trade debtor identifier
  name: debtorId
  type: string
- description: Total amount to claim
  name: claimAmount
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Date when the financial loss occurred
  name: lossDate
  type: string
- description: Customer invoice reference
  name: invoiceReference
  type: string
- description: Related payment overdue identifier
  name: overdueId
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-claims-submit_claim_request-schema.json
slug: trade-claims-submit_claim_request
source_filename: trade-claims-submit_claim_request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-claims-submit_claim_request-schema.json\",\n  \"title\": \"SubmitClaimRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for submitting an insurance claim\",\n  \"properties\": {\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Trade credit insurance policy identifier\"\n    },\n    \"debtorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the defaulting debtor\"\n    },\n    \"debtorId\": {\n      \"type\": \"string\",\n      \"description\": \"Allianz Trade debtor identifier\"\n    },\n    \"claimAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total amount to claim\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"lossDate\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date\",\n      \"description\": \"Date when the financial loss occurred\"\n    },\n    \"invoiceReference\": {\n      \"type\": \"string\",\n      \"description\": \"Customer invoice reference\"\n    },\n    \"overdueId\": {\n      \"type\": \"string\",\n      \"description\": \"Related payment overdue identifier\"\n    }\n  },\n  \"required\": [\n    \"policyId\",\n    \"debtorName\",\n    \"claimAmount\",\n    \"currency\",\n    \"lossDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-claims-submit_claim_request-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: SubmitClaimRequest
---
