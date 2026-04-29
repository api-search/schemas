---
description: ''
layout: schema
name: SuccessfulGetJobInfoQuery
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: operation
  type: string
- description: ''
  name: object
  type: string
- description: ''
  name: createdById
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: systemModstamp
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: concurrencyMode
  type: string
- description: ''
  name: contentType
  type: string
- description: ''
  name: apiVersion
  type: integer
- description: ''
  name: jobType
  type: string
- description: ''
  name: retries
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
schema_file: json-schema/salesforce-successful-get-job-info-query-schema.json
slug: salesforce-successful-get-job-info-query
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"createdById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"systemModstamp\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"concurrencyMode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"apiVersion\": {\n      \"type\": \"integer\",\n      \"example\": 10\n\
  \    },\n    \"jobType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"retries\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"totalProcessingTime\": {\n      \"type\": \"integer\",\n      \"example\": 1700000000000\n    },\n    \"apiActiveProcessingTime\": {\n      \"type\": \"integer\",\n      \"example\": 1700000000000\n    },\n    \"apexProcessingTime\": {\n      \"type\": \"integer\",\n      \"example\": 1700000000000\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"operation\",\n    \"object\",\n    \"createdById\",\n    \"createdDate\",\n    \"systemModstamp\",\n    \"state\",\n    \"concurrencyMode\",\n    \"contentType\",\n    \"apiVersion\",\n    \"jobType\",\n    \"retries\",\n    \"totalProcessingTime\",\n    \"apiActiveProcessingTime\",\n    \"apexProcessingTime\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulGetJobInfoQuery\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-get-job-info-query-schema.json
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
title: SuccessfulGetJobInfoQuery
---
