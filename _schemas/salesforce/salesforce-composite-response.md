---
description: ''
layout: schema
name: CompositeResponse
properties_list:
- description: ''
  name: body
  type: object
- description: ''
  name: httpHeaders
  type: object
- description: ''
  name: httpStatusCode
  type: integer
- description: ''
  name: referenceId
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-composite-response-schema.json
slug: salesforce-composite-response
source_filename: salesforce-composite-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"success\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"errors\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"success\",\n        \"errors\"\n      ]\n    },\n    \"httpHeaders\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Location\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"Location\"\n      ]\n    },\n    \"httpStatusCode\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"referenceId\"\
  : {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"body\",\n    \"httpHeaders\",\n    \"httpStatusCode\",\n    \"referenceId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompositeResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-composite-response-schema.json
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
title: CompositeResponse
---
