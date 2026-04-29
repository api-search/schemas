---
description: ''
layout: schema
name: Accounts
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: errors
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-accounts-schema.json
slug: salesforce-accounts
source_filename: salesforce-accounts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"uiapi\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"query\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Account\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"edges\": {\n                      \"type\": \"array\",\n                      \"description\": \"\",\n                      \"example\": [],\n                      \"items\": {\n                        \"type\": \"object\"\n                      }\n                    }\n                  },\n                  \"required\": [\n                    \"edges\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"Account\"\n              ]\n            }\n          },\n          \"required\": [\n    \
  \        \"query\"\n          ]\n        }\n      },\n      \"required\": [\n        \"uiapi\"\n      ]\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"data\",\n    \"errors\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Accounts\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-accounts-schema.json
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
title: Accounts
---
