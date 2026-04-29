---
description: ''
layout: schema
name: Page
properties_list:
- description: ''
  name: currentPageToken
  type: integer
- description: ''
  name: currentPageUrl
  type: string
- description: ''
  name: items
  type: array
- description: ''
  name: nextPageToken
  type: '[''string'', ''null'']'
- description: ''
  name: nextPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: previousPageToken
  type: '[''string'', ''null'']'
- description: ''
  name: previousPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: total
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-page-schema.json
slug: salesforce-page
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentPageToken\": {\n      \"type\": \"integer\",\n      \"example\": \"CAUQAA\"\n    },\n    \"currentPageUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"nextPageToken\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"CAUQAA\"\n    },\n    \"nextPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"previousPageToken\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"CAUQAA\"\n    },\n    \"previousPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    }\n  },\n  \"required\":\
  \ [\n    \"currentPageToken\",\n    \"currentPageUrl\",\n    \"items\",\n    \"nextPageToken\",\n    \"nextPageUrl\",\n    \"previousPageToken\",\n    \"previousPageUrl\",\n    \"total\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Page\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-page-schema.json
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
title: Page
---
