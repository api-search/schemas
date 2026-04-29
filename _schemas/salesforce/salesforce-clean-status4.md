---
description: ''
layout: schema
name: CleanStatus4
properties_list:
- description: ''
  name: controllerValues
  type: object
- description: ''
  name: defaultValue
  type: '[''string'', ''null'']'
- description: ''
  name: eTag
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: values
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-clean-status4-schema.json
slug: salesforce-clean-status4
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"controllerValues\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"defaultValue\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"eTag\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"validFor\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n  \
  \          \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"attributes\",\n          \"label\",\n          \"validFor\",\n          \"value\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"controllerValues\",\n    \"defaultValue\",\n    \"eTag\",\n    \"url\",\n    \"values\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CleanStatus4\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-clean-status4-schema.json
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
title: CleanStatus4
---
