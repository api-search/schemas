---
description: ''
layout: schema
name: CreateSandbox
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: success
  type: boolean
- description: ''
  name: errors
  type: array
- description: ''
  name: warnings
  type: array
- description: ''
  name: infos
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-create-sandbox-schema.json
slug: salesforce-create-sandbox
source_filename: salesforce-create-sandbox-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"infos\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"success\",\n    \"errors\",\n    \"warnings\",\n    \"infos\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateSandbox\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-create-sandbox-schema.json
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
title: CreateSandbox
---
