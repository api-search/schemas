---
description: ''
layout: schema
name: TestCase
properties_list:
- description: ''
  name: endTime
  type: string
- description: ''
  name: generatedData
  type: object
- description: ''
  name: inputs
  type: object
- description: ''
  name: startTime
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: testNumber
  type: integer
- description: ''
  name: testResults
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-test-case-schema.json
slug: salesforce-test-case
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"generatedData\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"actionsSequence\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"invokedActions\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"outcome\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"sessionId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"topic\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"citations\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"actionsSequence\",\n        \"invokedActions\"\
  ,\n        \"outcome\",\n        \"sessionId\",\n        \"topic\"\n      ]\n    },\n    \"inputs\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"contextVariables\": {\n          \"type\": \"object\",\n          \"example\": \"example_value\"\n        },\n        \"conversationHistory\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"utterance\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"contextVariables\",\n        \"conversationHistory\",\n        \"utterance\"\n      ]\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"testNumber\": {\n      \"type\": \"integer\",\n      \"\
  example\": 10\n    },\n    \"testResults\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"actualValue\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"endTime\": {\n            \"type\": \"string\",\n            \"example\": \"2026-01-15T10:30:00Z\"\n          },\n          \"errorCode\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"expectedValue\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"metricLabel\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"result\": {\n            \"type\": \"string\",\n            \"\
  example\": \"example_value\"\n          },\n          \"score\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"startTime\": {\n            \"type\": \"string\",\n            \"example\": \"2026-01-15T10:30:00Z\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"metricExplainability\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"endTime\",\n          \"errorCode\",\n          \"metricLabel\",\n          \"name\",\n          \"score\",\n          \"startTime\",\n          \"status\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"endTime\",\n    \"generatedData\",\n    \"inputs\",\n    \"startTime\",\n    \"status\",\n    \"testNumber\",\n    \"testResults\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\"\
  : \"TestCase\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-test-case-schema.json
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
title: TestCase
---
