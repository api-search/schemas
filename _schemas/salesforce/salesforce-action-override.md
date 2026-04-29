---
description: ''
layout: schema
name: ActionOverride
properties_list:
- description: ''
  name: formFactor
  type: string
- description: ''
  name: isAvailableInTouch
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: pageId
  type: string
- description: ''
  name: url
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-action-override-schema.json
slug: salesforce-action-override
source_filename: salesforce-action-override-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"formFactor\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"isAvailableInTouch\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"pageId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"url\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"formFactor\",\n    \"isAvailableInTouch\",\n    \"name\",\n    \"pageId\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActionOverride\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-action-override-schema.json
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
title: ActionOverride
---
