---
description: Request body for reporting a payment overdue
layout: schema
name: ReportOverdueRequest
properties_list:
- description: Trade credit insurance policy identifier
  name: policyId
  type: string
- description: Overdue category type code
  name: overdueCategoryTypeCode
  type: string
- description: Name of the debtor
  name: debtorName
  type: string
- description: Allianz Trade debtor identifier
  name: debtorId
  type: string
- description: Amount overdue
  name: overdueAmount
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Original invoice due date
  name: dueDate
  type: string
- description: Customer invoice reference
  name: invoiceReference
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-payment-overdues-report_overdue_request-schema.json
slug: trade-payment-overdues-report_overdue_request
source_filename: trade-payment-overdues-report_overdue_request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-payment-overdues-report_overdue_request-schema.json\",\n  \"title\": \"ReportOverdueRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for reporting a payment overdue\",\n  \"properties\": {\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Trade credit insurance policy identifier\"\n    },\n    \"overdueCategoryTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Overdue category type code\",\n      \"enum\": [\n        \"OVD\",\n        \"EXP\",\n        \"RES\"\n      ]\n    },\n    \"debtorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the debtor\"\n    },\n    \"debtorId\": {\n      \"type\": \"string\",\n      \"description\": \"Allianz Trade debtor identifier\"\n    },\n    \"overdueAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n \
  \     \"description\": \"Amount overdue\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Original invoice due date\"\n    },\n    \"invoiceReference\": {\n      \"type\": \"string\",\n      \"description\": \"Customer invoice reference\"\n    }\n  },\n  \"required\": [\n    \"policyId\",\n    \"overdueCategoryTypeCode\",\n    \"debtorName\",\n    \"overdueAmount\",\n    \"currency\",\n    \"dueDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-payment-overdues-report_overdue_request-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: ReportOverdueRequest
---
