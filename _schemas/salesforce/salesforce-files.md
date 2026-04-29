---
description: ''
layout: schema
name: Files
properties_list:
- description: ''
  name: items
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-files-schema.json
slug: salesforce-files
source_filename: salesforce-files-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"items\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Files\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-files-schema.json
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
title: Files
---
