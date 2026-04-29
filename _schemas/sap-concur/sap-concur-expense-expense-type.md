---
description: An expense category classification
layout: schema
name: ExpenseType
properties_list:
- description: The expense type identifier (e.g., BRKFT, LODNG, AIRFR)
  name: id
  type: string
- description: The localized display name
  name: name
  type: string
- description: The expense type code
  name: code
  type: string
- description: Whether this type has been deactivated
  name: isDeleted
  type: boolean
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-expense-type-schema.json
slug: sap-concur-expense-expense-type
source_filename: sap-concur-expense-expense-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExpenseType\",\n  \"type\": \"object\",\n  \"description\": \"An expense category classification\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The expense type identifier (e.g., BRKFT, LODNG, AIRFR)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The localized display name\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The expense type code\"\n    },\n    \"isDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this type has been deactivated\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-expense-type-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ExpenseType
---
