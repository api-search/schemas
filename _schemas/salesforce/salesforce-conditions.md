---
description: ''
layout: schema
name: Conditions
properties_list:
- description: ''
  name: conditionsList
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-conditions-schema.json
slug: salesforce-conditions
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"conditionsList\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"value\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          }\n        },\n        \"required\": [\n          \"fieldName\",\n          \"value\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"conditionsList\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Conditions\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-conditions-schema.json
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
title: Conditions
---
