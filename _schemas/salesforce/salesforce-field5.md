---
description: ''
layout: schema
name: Field5
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: object
- description: ''
  name: doc
  type: string
- description: ''
  name: default
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-field5-schema.json
slug: salesforce-field5
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"type\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"doc\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"default\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Field5\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-field5-schema.json
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
title: Field5
---
