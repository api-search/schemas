---
description: ''
layout: schema
name: GetParallelResultsforaQueryJob
properties_list:
- description: ''
  name: resultPages
  type: array
- description: ''
  name: nextRecordsUrl
  type: string
- description: ''
  name: done
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-parallel-resultsfora-query-job-schema.json
slug: salesforce-get-parallel-resultsfora-query-job
source_filename: salesforce-get-parallel-resultsfora-query-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"resultPages\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"resultLink\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"resultLink\"\n        ]\n      }\n    },\n    \"nextRecordsUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"done\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"resultPages\",\n    \"nextRecordsUrl\",\n    \"done\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetParallelResultsforaQueryJob\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-parallel-resultsfora-query-job-schema.json
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
title: GetParallelResultsforaQueryJob
---
