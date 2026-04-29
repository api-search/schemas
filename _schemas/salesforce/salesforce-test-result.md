---
description: ''
layout: schema
name: TestResult
properties_list:
- description: ''
  name: actualValue
  type: string
- description: ''
  name: endTime
  type: string
- description: ''
  name: errorCode
  type: integer
- description: ''
  name: expectedValue
  type: string
- description: ''
  name: metricLabel
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: result
  type: string
- description: ''
  name: score
  type: integer
- description: ''
  name: startTime
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: metricExplainability
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-test-result-schema.json
slug: salesforce-test-result
source_filename: salesforce-test-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"actualValue\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"errorCode\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"expectedValue\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"metricLabel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"score\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n\
  \    },\n    \"metricExplainability\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"endTime\",\n    \"errorCode\",\n    \"metricLabel\",\n    \"name\",\n    \"score\",\n    \"startTime\",\n    \"status\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TestResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-test-result-schema.json
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
title: TestResult
---
