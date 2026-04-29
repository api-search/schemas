---
description: ''
layout: schema
name: DeleteAccount
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: errors
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-delete-account-schema.json
slug: salesforce-delete-account
source_filename: salesforce-delete-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"uiapi\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"AccountDelete\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Id\": {\n                  \"type\": \"string\",\n                  \"example\": \"abc123\"\n                }\n              },\n              \"required\": [\n                \"Id\"\n              ]\n            }\n          },\n          \"required\": [\n            \"AccountDelete\"\n          ]\n        }\n      },\n      \"required\": [\n        \"uiapi\"\n      ]\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"data\",\n    \"errors\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"DeleteAccount\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-delete-account-schema.json
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
title: DeleteAccount
---
