---
description: ''
layout: schema
name: ToolingExecuteAnonymous
properties_list:
- description: ''
  name: line
  type: integer
- description: ''
  name: column
  type: integer
- description: ''
  name: compiled
  type: boolean
- description: ''
  name: success
  type: boolean
- description: ''
  name: compileProblem
  type: '[''string'', ''null'']'
- description: ''
  name: exceptionStackTrace
  type: '[''string'', ''null'']'
- description: ''
  name: exceptionMessage
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-tooling-execute-anonymous-schema.json
slug: salesforce-tooling-execute-anonymous
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"line\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"column\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"compiled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"compileProblem\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"exceptionStackTrace\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"exceptionMessage\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"line\",\n    \"column\",\n    \"compiled\",\n    \"success\",\n    \"compileProblem\",\n    \"exceptionStackTrace\",\n    \"exceptionMessage\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ToolingExecuteAnonymous\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-tooling-execute-anonymous-schema.json
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
title: ToolingExecuteAnonymous
---
