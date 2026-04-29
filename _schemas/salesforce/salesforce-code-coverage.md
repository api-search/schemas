---
description: ''
layout: schema
name: CodeCoverage
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: locationsNotCovered
  type: array
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: '[''string'', ''null'']'
- description: ''
  name: numLocations
  type: integer
- description: ''
  name: numLocationsNotCovered
  type: integer
- description: ''
  name: type
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-code-coverage-schema.json
slug: salesforce-code-coverage
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"locationsNotCovered\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"namespace\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"numLocations\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"numLocationsNotCovered\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"locationsNotCovered\",\n    \"name\",\n    \"namespace\",\n    \"numLocations\",\n    \"numLocationsNotCovered\",\n    \"type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"CodeCoverage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-code-coverage-schema.json
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
title: CodeCoverage
---
