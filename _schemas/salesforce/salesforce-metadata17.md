---
description: ''
layout: schema
name: Metadata17
properties_list:
- description: ''
  name: apiVersion
  type: integer
- description: ''
  name: packageVersions
  type: array
- description: ''
  name: status
  type: string
- description: ''
  name: urls
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-metadata17-schema.json
slug: salesforce-metadata17
source_filename: salesforce-metadata17-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"packageVersions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"urls\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"apiVersion\",\n    \"packageVersions\",\n    \"status\",\n    \"urls\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metadata17\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-metadata17-schema.json
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
title: Metadata17
---
