---
description: ''
layout: schema
name: CreateAccountSuccess
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: errors
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-create-account-success-schema.json
slug: salesforce-create-account-success
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"uiapi\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"AccountCreate\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Record\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"Id\": {\n                      \"type\": \"string\",\n                      \"example\": \"abc123\"\n                    },\n                    \"Name\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"value\": {\n                          \"type\": \"object\"\n                        }\n                      },\n                      \"required\": [\n                        \"value\"\n                      ]\n                    }\n                  },\n                  \"required\"\
  : [\n                    \"Id\",\n                    \"Name\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"Record\"\n              ]\n            }\n          },\n          \"required\": [\n            \"AccountCreate\"\n          ]\n        }\n      },\n      \"required\": [\n        \"uiapi\"\n      ]\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"data\",\n    \"errors\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateAccountSuccess\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-create-account-success-schema.json
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
title: CreateAccountSuccess
---
