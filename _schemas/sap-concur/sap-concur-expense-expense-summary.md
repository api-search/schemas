---
description: A summary of an expense entry on a report
layout: schema
name: ExpenseSummary
properties_list:
- description: Unique identifier of the expense
  name: expenseId
  type: string
- description: The date the transaction occurred
  name: transactionDate
  type: string
- description: Business justification for this expense
  name: businessPurpose
  type: string
- description: ''
  name: links
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-expense-summary-schema.json
slug: sap-concur-expense-expense-summary
source_filename: sap-concur-expense-expense-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExpenseSummary\",\n  \"type\": \"object\",\n  \"description\": \"A summary of an expense entry on a report\",\n  \"properties\": {\n    \"expenseId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the expense\"\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date the transaction occurred\"\n    },\n    \"businessPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"Business justification for this expense\"\n    },\n    \"links\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-expense-summary-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ExpenseSummary
---
