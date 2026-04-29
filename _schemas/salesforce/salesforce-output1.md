---
description: ''
layout: schema
name: Output1
properties_list:
- description: ''
  name: error
  type: string
- description: ''
  name: results
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-output1-schema.json
slug: salesforce-output1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"error\",\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Output1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-output1-schema.json
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
title: Output1
---
