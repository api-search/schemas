---
description: ''
layout: schema
name: SuccessfulFollowing
properties_list:
- description: ''
  name: currentPageUrl
  type: string
- description: ''
  name: following
  type: array
- description: ''
  name: nextPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: previousPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: total
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-following-schema.json
slug: salesforce-successful-following
source_filename: salesforce-successful-following-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentPageUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"following\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"nextPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"previousPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    }\n  },\n  \"required\": [\n    \"currentPageUrl\",\n    \"following\",\n    \"nextPageUrl\",\n    \"previousPageUrl\",\n    \"total\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulFollowing\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-following-schema.json
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
title: SuccessfulFollowing
---
