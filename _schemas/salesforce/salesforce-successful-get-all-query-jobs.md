---
description: ''
layout: schema
name: SuccessfulGetAllQueryJobs
properties_list:
- description: ''
  name: done
  type: boolean
- description: ''
  name: nextRecordsUrl
  type: '[''string'', ''null'']'
- description: ''
  name: records
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-get-all-query-jobs-schema.json
slug: salesforce-successful-get-all-query-jobs
source_filename: salesforce-successful-get-all-query-jobs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"done\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"nextRecordsUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"operation\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"object\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"createdById\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"createdDate\": {\n            \"type\": \"string\",\n            \"example\": \"\
  example_value\"\n          },\n          \"systemModstamp\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"concurrencyMode\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"contentType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"apiVersion\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"jobType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"operation\",\n          \"object\",\n          \"createdById\",\n          \"createdDate\",\n          \"systemModstamp\",\n          \"state\",\n          \"concurrencyMode\",\n   \
  \       \"contentType\",\n          \"apiVersion\",\n          \"jobType\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"done\",\n    \"nextRecordsUrl\",\n    \"records\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulGetAllQueryJobs\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-get-all-query-jobs-schema.json
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
title: SuccessfulGetAllQueryJobs
---
