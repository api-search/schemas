---
description: ''
layout: schema
name: TransactionHistoryRequest
properties_list:
- description: ''
  name: membershipNumber
  type: string
- description: ''
  name: journalType
  type: string
- description: ''
  name: journalSubType
  type: string
- description: ''
  name: periodStartDate
  type: string
- description: ''
  name: periodEndDate
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-transaction-history-request-schema.json
slug: salesforce-transaction-history-request
source_filename: salesforce-transaction-history-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"membershipNumber\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"journalType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"journalSubType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"periodStartDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"periodEndDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"membershipNumber\",\n    \"journalType\",\n    \"journalSubType\",\n    \"periodStartDate\",\n    \"periodEndDate\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionHistoryRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-transaction-history-request-schema.json
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
title: TransactionHistoryRequest
---
