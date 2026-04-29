---
description: ''
layout: schema
name: Status201-Success4
properties_list:
- description: ''
  name: code
  type: string
- description: ''
  name: decisionTable
  type: object
- description: ''
  name: isSuccess
  type: boolean
- description: ''
  name: message
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status201-success4-schema.json
slug: salesforce-status201-success4
source_filename: salesforce-status201-success4-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"decisionTable\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"parameters\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"sourceCriteria\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"parameters\",\n        \"sourceCriteria\"\n      ]\n    },\n    \"isSuccess\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"message\": {\n      \"type\": \"string\",\n  \
  \    \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"decisionTable\",\n    \"isSuccess\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status201-Success4\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status201-success4-schema.json
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
title: Status201-Success4
---
