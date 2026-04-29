---
description: ''
layout: schema
name: Status201-BadRequest
properties_list:
- description: ''
  name: errors
  type: array
- description: ''
  name: message
  type: string
- description: ''
  name: success
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status201-bad-request-schema.json
slug: salesforce-status201-bad-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"errorCode\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"errorMessage\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"recordId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"errorCode\",\n          \"errorMessage\",\n          \"recordId\"\n        ]\n      }\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"errors\",\n    \"message\",\n    \"success\"\n  ],\n\
  \  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status201-BadRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status201-bad-request-schema.json
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
title: Status201-BadRequest
---
