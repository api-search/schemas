---
description: An individual expense entry.
layout: schema
name: Expense
properties_list:
- description: Unique identifier for the expense entry.
  name: expenseId
  type: string
- description: Name of the expense type.
  name: expenseTypeName
  type: string
- description: Date of the transaction.
  name: transactionDate
  type: string
- description: Amount of the transaction.
  name: transactionAmount
  type: number
- description: Currency code of the transaction.
  name: transactionCurrencyCode
  type: string
- description: Name of the vendor.
  name: vendorName
  type: string
- description: Description of the expense.
  name: description
  type: string
- description: Whether a receipt is required.
  name: receiptRequired
  type: boolean
provider_name: SAP Concur
provider_slug: concur
schema_file: json-schema/concur-expense-api-expense-schema.json
slug: concur-expense-api-expense
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/json-schema/concur-expense-api-expense-schema.json\",\n  \"title\": \"Expense\",\n  \"description\": \"An individual expense entry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expenseId\": { \"type\": \"string\", \"description\": \"Unique identifier for the expense entry.\", \"example\": \"600456\" },\n    \"expenseTypeName\": { \"type\": \"string\", \"description\": \"Name of the expense type.\", \"example\": \"Airfare\" },\n    \"transactionDate\": { \"type\": \"string\", \"format\": \"date\", \"description\": \"Date of the transaction.\" },\n    \"transactionAmount\": { \"type\": \"number\", \"format\": \"double\", \"description\": \"Amount of the transaction.\" },\n    \"transactionCurrencyCode\": { \"type\": \"string\", \"description\": \"Currency code of the transaction.\" },\n    \"vendorName\": { \"type\"\
  : \"string\", \"description\": \"Name of the vendor.\", \"example\": \"United Airlines\" },\n    \"description\": { \"type\": \"string\", \"description\": \"Description of the expense.\" },\n    \"receiptRequired\": { \"type\": \"boolean\", \"description\": \"Whether a receipt is required.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/json-schema/concur-expense-api-expense-schema.json
tags:
- Expense Management
- Finance
- Invoice
- SAP
- Travel
title: Expense
---
