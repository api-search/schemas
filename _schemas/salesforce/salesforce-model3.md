---
description: ''
layout: schema
name: Model3
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: quoteId
  type: string
- description: ''
  name: templateId
  type: string
- description: ''
  name: outputFormat
  type: string
- description: ''
  name: language
  type: string
- description: ''
  name: paperSize
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-model3-schema.json
slug: salesforce-model3
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"quoteId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"templateId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"outputFormat\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"paperSize\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"quoteId\",\n    \"templateId\",\n    \"outputFormat\",\n    \"language\",\n    \"paperSize\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Model3\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-model3-schema.json
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
title: Model3
---
