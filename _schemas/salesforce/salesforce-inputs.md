---
description: ''
layout: schema
name: Inputs
properties_list:
- description: ''
  name: contextVariables
  type: object
- description: ''
  name: conversationHistory
  type: array
- description: ''
  name: utterance
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-inputs-schema.json
slug: salesforce-inputs
source_filename: salesforce-inputs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"contextVariables\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"conversationHistory\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"utterance\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"contextVariables\",\n    \"conversationHistory\",\n    \"utterance\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Inputs\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-inputs-schema.json
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
title: Inputs
---
