---
description: An expense report submitted by a member
layout: schema
name: Expense
properties_list:
- description: Unique expense identifier
  name: id
  type: string
- description: ID of the member who submitted the expense
  name: member_id
  type: string
- description: Expense amount
  name: amount
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Expense category
  name: category
  type: string
- description: Description of the expense
  name: description
  type: string
- description: Date of the expense
  name: date
  type: string
- description: Current status of the expense
  name: status
  type: string
- description: URL to the uploaded receipt
  name: receipt_url
  type: string
- description: Timestamp when the expense was created
  name: created_at
  type: string
- description: Timestamp when the expense was last updated
  name: updated_at
  type: string
provider_name: Abacus
provider_slug: abacus
schema_file: json-schema/abacus-expense-schema.json
slug: abacus-expense
source_filename: abacus-expense-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-expense-schema.json\",\n  \"title\": \"Expense\",\n  \"description\": \"An expense report submitted by a member\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique expense identifier\",\n      \"example\": \"exp-500123\"\n    },\n    \"member_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the member who submitted the expense\",\n      \"example\": \"500123\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Expense amount\",\n      \"example\": 45.5\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\",\n      \"example\": \"USD\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Expense category\"\
  ,\n      \"enum\": [\n        \"meals\",\n        \"travel\",\n        \"lodging\",\n        \"office_supplies\",\n        \"software\",\n        \"other\"\n      ],\n      \"example\": \"meals\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the expense\",\n      \"example\": \"Team lunch\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the expense\",\n      \"example\": \"2025-03-15\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the expense\",\n      \"enum\": [\n        \"pending\",\n        \"approved\",\n        \"rejected\",\n        \"reimbursed\"\n      ],\n      \"example\": \"pending\"\n    },\n    \"receipt_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the uploaded receipt\",\n      \"example\": \"https://api.abacus.com/receipts/abc123\"\n    },\n\
  \    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the expense was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the expense was last updated\",\n      \"example\": \"2025-03-16T10:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-expense-schema.json
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
title: Expense
---
