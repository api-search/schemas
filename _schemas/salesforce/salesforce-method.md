---
description: ''
layout: schema
name: Method
properties_list:
- description: ''
  name: annotations
  type: array
- description: ''
  name: location
  type: object
- description: ''
  name: modifiers
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: references
  type: array
- description: ''
  name: returnType
  type: string
- description: ''
  name: type
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-method-schema.json
slug: salesforce-method
source_filename: salesforce-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotations\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"column\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"line\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"column\",\n        \"line\"\n      ]\n    },\n    \"modifiers\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"type\"\n        ]\n      }\n    },\n    \"references\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"returnType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"type\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"annotations\",\n    \"location\",\n    \"modifiers\",\n    \"name\",\n    \"parameters\",\n    \"references\",\n    \"returnType\",\n    \"type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\"\
  : \"Method\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-method-schema.json
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
title: Method
---
