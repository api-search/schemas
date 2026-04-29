---
description: ''
layout: schema
name: Body5
properties_list:
- description: ''
  name: messageSegments
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-body5-schema.json
slug: salesforce-body5
source_filename: salesforce-body5-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageSegments\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"text\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"markupType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          }\n        },\n        \"required\": [\n          \"type\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"messageSegments\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Body5\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-body5-schema.json
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
title: Body5
---
