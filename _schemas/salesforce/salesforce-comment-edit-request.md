---
description: ''
layout: schema
name: Comment-EditRequest
properties_list:
- description: ''
  name: body
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-comment-edit-request-schema.json
slug: salesforce-comment-edit-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"messageSegments\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"text\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"text\",\n              \"type\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"messageSegments\"\n      ]\n    }\n  },\n  \"required\": [\n    \"body\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Comment-EditRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-comment-edit-request-schema.json
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
title: Comment-EditRequest
---
