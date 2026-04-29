---
description: An insurance claim filed with Allianz Trade
layout: schema
name: Claim
properties_list:
- description: Unique identifier for the insurance claim
  name: claimId
  type: string
- description: Trade credit insurance policy identifier
  name: policyId
  type: string
- description: Name of the debtor who defaulted on payment
  name: debtorName
  type: string
- description: Allianz Trade debtor identifier
  name: debtorId
  type: string
- description: Total amount claimed
  name: claimAmount
  type: number
- description: Amount approved by Allianz Trade (after processing)
  name: approvedAmount
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Current status of the claim
  name: claimStatus
  type: string
- description: Date when the financial loss occurred
  name: lossDate
  type: string
- description: Customer invoice reference number
  name: invoiceReference
  type: string
- description: Related payment overdue identifier
  name: overdueId
  type: string
- description: Timestamp when the claim was submitted
  name: submittedAt
  type: string
- description: Timestamp when the claim was resolved
  name: resolvedAt
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-claims-claim-schema.json
slug: trade-claims-claim
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-claims-claim-schema.json\",\n  \"title\": \"Claim\",\n  \"type\": \"object\",\n  \"description\": \"An insurance claim filed with Allianz Trade\",\n  \"properties\": {\n    \"claimId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the insurance claim\"\n    },\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Trade credit insurance policy identifier\"\n    },\n    \"debtorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the debtor who defaulted on payment\"\n    },\n    \"debtorId\": {\n      \"type\": \"string\",\n      \"description\": \"Allianz Trade debtor identifier\"\n    },\n    \"claimAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total amount claimed\"\n    },\n    \"approvedAmount\": {\n      \"type\": \"number\"\
  ,\n      \"format\": \"double\",\n      \"description\": \"Amount approved by Allianz Trade (after processing)\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"claimStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the claim\",\n      \"enum\": [\n        \"submitted\",\n        \"under_review\",\n        \"approved\",\n        \"rejected\",\n        \"paid\"\n      ]\n    },\n    \"lossDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the financial loss occurred\"\n    },\n    \"invoiceReference\": {\n      \"type\": \"string\",\n      \"description\": \"Customer invoice reference number\"\n    },\n    \"overdueId\": {\n      \"type\": \"string\",\n      \"description\": \"Related payment overdue identifier\"\n    },\n    \"submittedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when the claim was submitted\"\n    },\n    \"resolvedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the claim was resolved\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-claims-claim-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: Claim
---
