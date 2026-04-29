---
description: ''
layout: schema
name: Status400-ExpressionNotFound1
properties_list:
- description: ''
  name: actionName
  type: string
- description: ''
  name: errors
  type: array
- description: ''
  name: isSuccess
  type: boolean
- description: ''
  name: outputValues
  type: '[''string'', ''null'']'
- description: ''
  name: version
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status400-expression-not-found1-schema.json
slug: salesforce-status400-expression-not-found1
source_filename: salesforce-status400-expression-not-found1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"statusCode\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"fields\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"required\": [\n          \"statusCode\",\n          \"message\",\n          \"fields\"\n        ]\n      }\n    },\n    \"isSuccess\": {\n      \"type\": \"boolean\",\n      \"example\"\
  : true\n    },\n    \"outputValues\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"actionName\",\n    \"errors\",\n    \"isSuccess\",\n    \"outputValues\",\n    \"version\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status400-ExpressionNotFound1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status400-expression-not-found1-schema.json
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
title: Status400-ExpressionNotFound1
---
