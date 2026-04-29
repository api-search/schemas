---
description: ''
layout: schema
name: batchInfo
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: jobId
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: systemModstamp
  type: string
- description: ''
  name: numberRecordsProcessed
  type: integer
- description: ''
  name: numberRecordsFailed
  type: integer
- description: ''
  name: totalProcessingTime
  type: integer
- description: ''
  name: apiActiveProcessingTime
  type: integer
- description: ''
  name: apexProcessingTime
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-batch-info-schema.json
slug: salesforce-batch-info
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"jobId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"systemModstamp\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"numberRecordsProcessed\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"numberRecordsFailed\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"totalProcessingTime\": {\n      \"type\": \"integer\",\n      \"example\": 1700000000000\n    },\n    \"apiActiveProcessingTime\": {\n      \"type\": \"integer\",\n      \"example\": 1700000000000\n    },\n    \"apexProcessingTime\": {\n      \"type\": \"integer\",\n      \"example\"\
  : 1700000000000\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"jobId\",\n    \"state\",\n    \"createdDate\",\n    \"systemModstamp\",\n    \"numberRecordsProcessed\",\n    \"numberRecordsFailed\",\n    \"totalProcessingTime\",\n    \"apiActiveProcessingTime\",\n    \"apexProcessingTime\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"batchInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-batch-info-schema.json
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
title: batchInfo
---
