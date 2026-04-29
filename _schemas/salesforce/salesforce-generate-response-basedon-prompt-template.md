---
description: ''
layout: schema
name: GenerateResponseBasedonPromptTemplate
properties_list:
- description: ''
  name: generations
  type: array
- description: ''
  name: parameters
  type: '[''string'', ''null'']'
- description: ''
  name: prompt
  type: string
- description: ''
  name: promptTemplateDevName
  type: string
- description: ''
  name: requestId
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-generate-response-basedon-prompt-template-schema.json
slug: salesforce-generate-response-basedon-prompt-template
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"generations\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"parameters\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"responseId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"text\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"parameters\",\n          \"responseId\",\n          \"text\"\n        ]\n      }\n    },\n    \"parameters\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"promptTemplateDevName\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"example_value\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"generations\",\n    \"parameters\",\n    \"prompt\",\n    \"promptTemplateDevName\",\n    \"requestId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GenerateResponseBasedonPromptTemplate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-generate-response-basedon-prompt-template-schema.json
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
title: GenerateResponseBasedonPromptTemplate
---
