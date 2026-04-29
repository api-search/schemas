---
description: ''
layout: schema
name: TableDeclaration
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
  name: references
  type: array
- description: ''
  name: type
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-table-declaration-schema.json
slug: salesforce-table-declaration
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotations\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"name\"\n        ]\n      }\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"column\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"line\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"column\",\n        \"line\"\n      ]\n    },\n    \"modifiers\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"type\"\
  : \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"references\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"annotations\",\n    \"location\",\n    \"modifiers\",\n    \"name\",\n    \"references\",\n    \"type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableDeclaration\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-table-declaration-schema.json
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
title: TableDeclaration
---
