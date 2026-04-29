---
description: ''
layout: schema
name: CodeCoverageWarning
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: name
  type: '[''string'', ''null'']'
- description: ''
  name: namespace
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-code-coverage-warning-schema.json
slug: salesforce-code-coverage-warning
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"Example Title\"\n    },\n    \"namespace\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"message\",\n    \"name\",\n    \"namespace\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CodeCoverageWarning\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-code-coverage-warning-schema.json
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
title: CodeCoverageWarning
---
