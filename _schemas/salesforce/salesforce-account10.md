---
description: ''
layout: schema
name: Account10
properties_list:
- description: ''
  name: edges
  type: array
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: pageInfo
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-account10-schema.json
slug: salesforce-account10
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"edges\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"node\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              },\n              \"Name\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"value\"\n                ]\n              }\n            },\n            \"required\": [\n              \"Id\",\n              \"Name\"\n            ]\n          }\n        },\n        \"required\": [\n          \"node\"\n    \
  \    ]\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"pageInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"hasNextPage\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"hasPreviousPage\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"startCursor\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"endCursor\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"hasNextPage\",\n        \"hasPreviousPage\",\n        \"startCursor\",\n        \"endCursor\"\n      ]\n    }\n  },\n  \"required\": [\n    \"edges\",\n    \"totalCount\",\n    \"pageInfo\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Account10\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-account10-schema.json
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
title: Account10
---
