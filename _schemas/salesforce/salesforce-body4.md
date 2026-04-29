---
description: ''
layout: schema
name: Body4
properties_list:
- description: ''
  name: isRichText
  type: boolean
- description: ''
  name: messageSegments
  type: array
- description: ''
  name: text
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-body4-schema.json
slug: salesforce-body4
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"isRichText\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"messageSegments\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"text\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"text\",\n          \"type\"\n        ]\n      }\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"isRichText\",\n    \"messageSegments\",\n    \"text\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Body4\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-body4-schema.json
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
title: Body4
---
