---
description: ''
layout: schema
name: Variable
properties_list:
- description: ''
  name: collection
  type: boolean
- description: ''
  name: dataType
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: input
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: output
  type: boolean
- description: ''
  name: type
  type: string
- description: ''
  name: value
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-variable-schema.json
slug: salesforce-variable
source_filename: salesforce-variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"collection\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    },\n    \"input\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"output\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"collection\",\n    \"dataType\",\n    \"description\",\n    \"input\",\n    \"name\",\n    \"output\",\n    \"type\",\n    \"value\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"Variable\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-variable-schema.json
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
title: Variable
---
