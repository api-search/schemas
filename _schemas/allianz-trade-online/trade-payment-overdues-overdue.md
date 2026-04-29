---
description: A payment overdue reported to Allianz Trade
layout: schema
name: Overdue
properties_list:
- description: Unique identifier for the payment overdue
  name: overdueId
  type: string
- description: Trade credit insurance policy identifier
  name: policyId
  type: string
- description: Overdue category code (OVD=default, EXP=extension, RES=rescheduling)
  name: overdueCategoryTypeCode
  type: string
- description: Name of the debtor with the payment overdue
  name: debtorName
  type: string
- description: Allianz Trade debtor identifier
  name: debtorId
  type: string
- description: Amount overdue in the policy currency
  name: overdueAmount
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Original invoice due date
  name: dueDate
  type: string
- description: Customer invoice reference number
  name: invoiceReference
  type: string
- description: Current status of the overdue report
  name: status
  type: string
- description: Timestamp when the overdue was reported
  name: reportedAt
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-payment-overdues-overdue-schema.json
slug: trade-payment-overdues-overdue
source_filename: trade-payment-overdues-overdue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-payment-overdues-overdue-schema.json\",\n  \"title\": \"Overdue\",\n  \"type\": \"object\",\n  \"description\": \"A payment overdue reported to Allianz Trade\",\n  \"properties\": {\n    \"overdueId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the payment overdue\"\n    },\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Trade credit insurance policy identifier\"\n    },\n    \"overdueCategoryTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Overdue category code (OVD=default, EXP=extension, RES=rescheduling)\",\n      \"enum\": [\n        \"OVD\",\n        \"EXP\",\n        \"RES\"\n      ]\n    },\n    \"debtorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the debtor with the payment overdue\"\n    },\n    \"debtorId\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Allianz Trade debtor identifier\"\n    },\n    \"overdueAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Amount overdue in the policy currency\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Original invoice due date\"\n    },\n    \"invoiceReference\": {\n      \"type\": \"string\",\n      \"description\": \"Customer invoice reference number\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the overdue report\",\n      \"enum\": [\n        \"reported\",\n        \"processed\",\n        \"closed\"\n      ]\n    },\n    \"reportedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the overdue was reported\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-payment-overdues-overdue-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: Overdue
---
