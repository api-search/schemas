---
description: ''
layout: schema
name: Topics2
properties_list:
- description: ''
  name: canAssignTopics
  type: boolean
- description: ''
  name: items
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-topics2-schema.json
slug: salesforce-topics2
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"canAssignTopics\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"canAssignTopics\",\n    \"items\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Topics2\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-topics2-schema.json
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
title: Topics2
---
