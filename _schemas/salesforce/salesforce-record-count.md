---
description: ''
layout: schema
name: RecordCount
properties_list:
- description: ''
  name: sObjects
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record-count-schema.json
slug: salesforce-record-count
source_filename: salesforce-record-count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"sObjects\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"count\": {\n            \"type\": \"integer\",\n            \"example\": 42\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"count\",\n          \"name\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"sObjects\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecordCount\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record-count-schema.json
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
title: RecordCount
---
