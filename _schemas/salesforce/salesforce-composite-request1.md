---
description: ''
layout: schema
name: CompositeRequest1
properties_list:
- description: ''
  name: method
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: referenceId
  type: string
- description: ''
  name: body
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-composite-request1-schema.json
slug: salesforce-composite-request1
source_filename: salesforce-composite-request1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"method\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"referenceId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"body\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"LastName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"AccountId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"method\",\n    \"url\",\n    \"referenceId\",\n    \"body\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompositeRequest1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-composite-request1-schema.json
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
title: CompositeRequest1
---
