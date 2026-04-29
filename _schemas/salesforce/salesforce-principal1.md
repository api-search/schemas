---
description: ''
layout: schema
name: Principal1
properties_list:
- description: ''
  name: authenticationStatus
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: principalAccess
  type: array
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
schema_file: json-schema/salesforce-principal1-schema.json
slug: salesforce-principal1
source_filename: salesforce-principal1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"principalAccess\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"principalName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"principalType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sequenceNumber\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"authenticationStatus\",\n    \"id\",\n    \"parameters\",\n    \"principalAccess\"\
  ,\n    \"principalName\",\n    \"principalType\",\n    \"sequenceNumber\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Principal1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-principal1-schema.json
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
title: Principal1
---
