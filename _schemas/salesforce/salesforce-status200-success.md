---
description: ''
layout: schema
name: Status200-Success
properties_list:
- description: ''
  name: code
  type: string
- description: ''
  name: decisionTable
  type: object
- description: ''
  name: isSuccess
  type: boolean
- description: ''
  name: message
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status200-success-schema.json
slug: salesforce-status200-success
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"decisionTable\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"conditionCriteria\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"conditionType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"example\": \"A sample description.\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"parameters\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"fieldName\": {\n                \"type\": \"string\",\n                \"example\"\
  : \"example_value\"\n              },\n              \"isGroupByField\": {\n                \"type\": \"boolean\",\n                \"example\": true\n              },\n              \"operator\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"sequence\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              },\n              \"usage\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"fieldName\",\n              \"isGroupByField\",\n              \"usage\"\n            ]\n          }\n        },\n        \"setupName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"sourceCriteria\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n   \
  \         \"type\": \"string\"\n          }\n        },\n        \"sourceObject\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"conditionCriteria\",\n        \"conditionType\",\n        \"description\",\n        \"id\",\n        \"parameters\",\n        \"setupName\",\n        \"sourceCriteria\",\n        \"sourceObject\",\n        \"status\"\n      ]\n    },\n    \"isSuccess\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"decisionTable\",\n    \"isSuccess\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status200-Success\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status200-success-schema.json
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
title: Status200-Success
---
