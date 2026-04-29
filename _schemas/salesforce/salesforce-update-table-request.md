---
description: ''
layout: schema
name: UpdateTableRequest
properties_list:
- description: ''
  name: setupName
  type: string
- description: ''
  name: fullName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: usageType
  type: string
- description: ''
  name: sourceType
  type: string
- description: ''
  name: sourceObject
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: decisionResultPolicy
  type: string
- description: ''
  name: collectOperator
  type: string
- description: ''
  name: conditionType
  type: string
- description: ''
  name: conditionCriteria
  type: string
- description: ''
  name: parameters
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-update-table-request-schema.json
slug: salesforce-update-table-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"setupName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"fullName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    },\n    \"usageType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sourceType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sourceObject\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"decisionResultPolicy\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"collectOperator\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"conditionType\": {\n      \"type\"\
  : \"string\",\n      \"example\": \"example_value\"\n    },\n    \"conditionCriteria\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"usage\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"operator\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"sequence\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"fieldName\",\n          \"usage\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"setupName\",\n    \"fullName\",\n\
  \    \"description\",\n    \"usageType\",\n    \"sourceType\",\n    \"sourceObject\",\n    \"status\",\n    \"decisionResultPolicy\",\n    \"collectOperator\",\n    \"conditionType\",\n    \"conditionCriteria\",\n    \"parameters\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateTableRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-update-table-request-schema.json
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
title: UpdateTableRequest
---
