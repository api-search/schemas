---
description: ''
layout: schema
name: ExpenseReport
properties_list:
- description: ''
  name: userId
  type: string
- description: ''
  name: summary
  type: object
- description: ''
  name: categories
  type: array
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/expensereport.json
slug: expensereport
source_filename: expensereport.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/expensereport.json\",\n  \"title\": \"ExpenseReport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\"\n    },\n    \"summary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"totalMonthly\": {\n          \"type\": \"number\"\n        }\n      }\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"category\": {\n            \"type\": \"string\"\n          },\n          \"amount\": {\n            \"type\": \"number\"\n          },\n          \"percentage\": {\n            \"type\": \"number\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/expensereport.json
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: ExpenseReport
---
