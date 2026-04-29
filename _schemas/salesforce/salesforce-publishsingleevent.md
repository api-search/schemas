---
description: ''
layout: schema
name: Publishsingleevent
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
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-publishsingleevent-schema.json
slug: salesforce-publishsingleevent
source_filename: salesforce-publishsingleevent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"statusCode\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"fields\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"required\": [\n          \"statusCode\",\n          \"message\",\n          \"fields\"\n        ]\n      }\n    }\n\
  \  },\n  \"required\": [\n    \"id\",\n    \"success\",\n    \"errors\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Publishsingleevent\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-publishsingleevent-schema.json
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
title: Publishsingleevent
---
