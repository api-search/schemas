---
description: An itemized line within a parent expense, representing a breakdown of the total amount.
layout: schema
name: ExpenseItemization
properties_list:
- description: Unique identifier of the itemization
  name: itemizationId
  type: string
- description: The parent expense identifier
  name: expenseId
  type: string
- description: The date of the itemized charge
  name: transactionDate
  type: string
- description: Purpose of this specific itemization
  name: businessPurpose
  type: string
- description: ''
  name: customData
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-expense-itemization-schema.json
slug: sap-concur-expense-expense-itemization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExpenseItemization\",\n  \"type\": \"object\",\n  \"description\": \"An itemized line within a parent expense, representing a breakdown of the total amount.\",\n  \"properties\": {\n    \"itemizationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the itemization\"\n    },\n    \"expenseId\": {\n      \"type\": \"string\",\n      \"description\": \"The parent expense identifier\"\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date of the itemized charge\"\n    },\n    \"businessPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"Purpose of this specific itemization\"\n    },\n    \"customData\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-expense-itemization-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ExpenseItemization
---
