---
description: ''
layout: schema
name: Topics
properties_list:
- description: ''
  name: currentPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: nextPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: topics
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-topics-schema.json
slug: salesforce-topics
source_filename: salesforce-topics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"nextPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"currentPageUrl\",\n    \"nextPageUrl\",\n    \"topics\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Topics\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-topics-schema.json
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
title: Topics
---
