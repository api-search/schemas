---
description: ''
layout: schema
name: Input1
properties_list:
- description: ''
  name: input
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-input1-schema.json
slug: salesforce-input1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"value\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"input\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Input1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-input1-schema.json
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
title: Input1
---
