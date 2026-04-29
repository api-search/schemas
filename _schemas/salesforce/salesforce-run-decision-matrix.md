---
description: ''
layout: schema
name: runDecisionMatrix
properties_list:
- description: ''
  name: actionName
  type: string
- description: ''
  name: errors
  type: '[''string'', ''null'']'
- description: ''
  name: isSuccess
  type: boolean
- description: ''
  name: outputValues
  type: object
- description: ''
  name: version
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-run-decision-matrix-schema.json
slug: salesforce-run-decision-matrix
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"errors\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"isSuccess\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"outputValues\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"myColumnOutput\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"myColumnOutput\"\n      ]\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"actionName\",\n    \"errors\",\n    \"isSuccess\",\n    \"outputValues\",\n    \"version\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"runDecisionMatrix\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-run-decision-matrix-schema.json
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
title: runDecisionMatrix
---
