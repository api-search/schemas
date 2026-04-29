---
description: ''
layout: schema
name: SuccessfulSObjectTree
properties_list:
- description: ''
  name: hasErrors
  type: boolean
- description: ''
  name: results
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-s-object-tree-schema.json
slug: salesforce-successful-s-object-tree
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"hasErrors\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"referenceId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          }\n        },\n        \"required\": [\n          \"referenceId\",\n          \"id\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"hasErrors\",\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulSObjectTree\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-s-object-tree-schema.json
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
title: SuccessfulSObjectTree
---
