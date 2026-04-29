---
description: Paginated list of expenses
layout: schema
name: ExpenseListResponse
properties_list:
- description: ''
  name: expenses
  type: array
- description: Total number of expenses
  name: total
  type: integer
- description: Current page number
  name: page
  type: integer
- description: Number of results per page
  name: per_page
  type: integer
provider_name: Abacus
provider_slug: abacus
schema_file: json-schema/abacus-expense-list-response-schema.json
slug: abacus-expense-list-response
source_filename: abacus-expense-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-expense-list-response-schema.json\",\n  \"title\": \"ExpenseListResponse\",\n  \"description\": \"Paginated list of expenses\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expenses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Expense\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of expenses\",\n      \"example\": 250\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\",\n      \"example\": 1\n    },\n    \"per_page\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results per page\",\n      \"example\": 25\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-expense-list-response-schema.json
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
title: ExpenseListResponse
---
