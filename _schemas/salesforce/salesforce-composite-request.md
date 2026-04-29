---
description: ''
layout: schema
name: CompositeRequest
properties_list:
- description: ''
  name: compositeRequest
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-composite-request-schema.json
slug: salesforce-composite-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"compositeRequest\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"method\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"referenceId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"body\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"LastName\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"AccountId\": {\n \
  \               \"type\": \"string\",\n                \"example\": \"500123\"\n              }\n            }\n          }\n        },\n        \"required\": [\n          \"method\",\n          \"url\",\n          \"referenceId\",\n          \"body\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"compositeRequest\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompositeRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-composite-request-schema.json
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
title: CompositeRequest
---
