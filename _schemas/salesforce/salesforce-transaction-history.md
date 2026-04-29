---
description: ''
layout: schema
name: TransactionHistory
properties_list:
- description: ''
  name: message
  type: '[''string'', ''null'']'
- description: ''
  name: status
  type: boolean
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: transactionJournals
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-transaction-history-schema.json
slug: salesforce-transaction-history
source_filename: salesforce-transaction-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"transactionJournals\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"message\",\n    \"status\",\n    \"totalCount\",\n    \"transactionJournals\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionHistory\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-transaction-history-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: TransactionHistory
---
