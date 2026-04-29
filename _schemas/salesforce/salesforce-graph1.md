---
description: ''
layout: schema
name: Graph1
properties_list:
- description: ''
  name: graphId
  type: string
- description: ''
  name: graphResponse
  type: object
- description: ''
  name: isSuccessful
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-graph1-schema.json
slug: salesforce-graph1
source_filename: salesforce-graph1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"graphResponse\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"compositeResponse\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"body\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"example\": \"abc123\"\n                  },\n                  \"success\": {\n                    \"type\": \"boolean\",\n                    \"example\": true\n                  },\n                  \"errors\": {\n                    \"type\": \"array\",\n                    \"description\": \"\",\n                    \"example\": [],\n                \
  \    \"items\": {\n                      \"type\": \"object\"\n                    }\n                  }\n                },\n                \"required\": [\n                  \"id\",\n                  \"success\",\n                  \"errors\"\n                ]\n              },\n              \"httpHeaders\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"Location\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"Location\"\n                ]\n              },\n              \"httpStatusCode\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              },\n              \"referenceId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              }\n            },\n            \"required\": [\n              \"body\",\n   \
  \           \"httpHeaders\",\n              \"httpStatusCode\",\n              \"referenceId\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"compositeResponse\"\n      ]\n    },\n    \"isSuccessful\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"graphId\",\n    \"graphResponse\",\n    \"isSuccessful\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Graph1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-graph1-schema.json
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
title: Graph1
---
