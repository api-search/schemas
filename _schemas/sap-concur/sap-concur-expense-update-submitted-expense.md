---
description: Limited-field update for an expense on a submitted report. Only accessible with Company JWT authentication.
layout: schema
name: UpdateSubmittedExpense
properties_list:
- description: Business justification, maximum 64 characters
  name: businessPurpose
  type: string
- description: The source system that created or modified the expense
  name: expenseSource
  type: string
- description: Whether to mark the expense as rejected
  name: isExpenseRejected
  type: boolean
- description: Whether a physical receipt has been received
  name: isPaperReceiptReceived
  type: boolean
- description: ''
  name: customData
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-update-submitted-expense-schema.json
slug: sap-concur-expense-update-submitted-expense
source_filename: sap-concur-expense-update-submitted-expense-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateSubmittedExpense\",\n  \"type\": \"object\",\n  \"description\": \"Limited-field update for an expense on a submitted report. Only accessible with Company JWT authentication.\",\n  \"properties\": {\n    \"businessPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"Business justification, maximum 64 characters\"\n    },\n    \"expenseSource\": {\n      \"type\": \"string\",\n      \"description\": \"The source system that created or modified the expense\"\n    },\n    \"isExpenseRejected\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to mark the expense as rejected\"\n    },\n    \"isPaperReceiptReceived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a physical receipt has been received\"\n    },\n    \"customData\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-update-submitted-expense-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: UpdateSubmittedExpense
---
