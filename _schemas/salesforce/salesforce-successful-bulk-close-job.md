---
description: ''
layout: schema
name: SuccessfulBulkCloseJob
properties_list:
- description: ''
  name: apexProcessingTime
  type: integer
- description: ''
  name: apiActiveProcessingTime
  type: integer
- description: ''
  name: apiVersion
  type: integer
- description: ''
  name: assignmentRuleId
  type: '[''string'', ''null'']'
- description: ''
  name: concurrencyMode
  type: string
- description: ''
  name: contentType
  type: string
- description: ''
  name: createdById
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: externalIdFieldName
  type: '[''string'', ''null'']'
- description: ''
  name: fastPathEnabled
  type: boolean
- description: ''
  name: id
  type: string
- description: ''
  name: numberBatchesCompleted
  type: integer
- description: ''
  name: numberBatchesFailed
  type: integer
- description: ''
  name: numberBatchesInProgress
  type: integer
- description: ''
  name: numberBatchesQueued
  type: integer
- description: ''
  name: numberBatchesTotal
  type: integer
- description: ''
  name: numberRecordsFailed
  type: integer
- description: ''
  name: numberRecordsProcessed
  type: integer
- description: ''
  name: numberRetries
  type: integer
- description: ''
  name: object
  type: string
- description: ''
  name: operation
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: systemModstamp
  type: string
- description: ''
  name: totalProcessingTime
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-bulk-close-job-schema.json
slug: salesforce-successful-bulk-close-job
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"apexProcessingTime\": {\n      \"type\": \"integer\",\n      \"example\": 1700000000000\n    },\n    \"apiActiveProcessingTime\": {\n      \"type\": \"integer\",\n      \"example\": 1700000000000\n    },\n    \"apiVersion\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"assignmentRuleId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"concurrencyMode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"createdById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"externalIdFieldName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"fastPathEnabled\"\
  : {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"numberBatchesCompleted\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"numberBatchesFailed\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"numberBatchesInProgress\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"numberBatchesQueued\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"numberBatchesTotal\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"numberRecordsFailed\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"numberRecordsProcessed\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"numberRetries\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"operation\"\
  : {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"systemModstamp\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"totalProcessingTime\": {\n      \"type\": \"integer\",\n      \"example\": 1700000000000\n    }\n  },\n  \"required\": [\n    \"apexProcessingTime\",\n    \"apiActiveProcessingTime\",\n    \"apiVersion\",\n    \"assignmentRuleId\",\n    \"concurrencyMode\",\n    \"contentType\",\n    \"createdById\",\n    \"createdDate\",\n    \"externalIdFieldName\",\n    \"fastPathEnabled\",\n    \"id\",\n    \"numberBatchesCompleted\",\n    \"numberBatchesFailed\",\n    \"numberBatchesInProgress\",\n    \"numberBatchesQueued\",\n    \"numberBatchesTotal\",\n    \"numberRecordsFailed\",\n    \"numberRecordsProcessed\",\n    \"numberRetries\",\n    \"object\",\n    \"operation\",\n    \"state\",\n    \"systemModstamp\",\n   \
  \ \"totalProcessingTime\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulBulkCloseJob\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-bulk-close-job-schema.json
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
title: SuccessfulBulkCloseJob
---
