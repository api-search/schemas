---
description: ''
layout: schema
name: Principal
properties_list:
- description: ''
  name: principalName
  type: string
- description: ''
  name: principalType
  type: string
- description: ''
  name: sequenceNumber
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-principal-schema.json
slug: salesforce-principal
source_filename: salesforce-principal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"principalName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"principalType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sequenceNumber\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"principalName\",\n    \"principalType\",\n    \"sequenceNumber\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Principal\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-principal-schema.json
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
title: Principal
---
