---
description: ''
layout: schema
name: GetListViewRecordsRequest
properties_list:
- description: ''
  name: fields
  type: array
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: sortBy
  type: array
- description: ''
  name: searchTerm
  type: string
- description: ''
  name: where
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-list-view-records-request-schema.json
slug: salesforce-get-list-view-records-request
source_filename: salesforce-get-list-view-records-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"sortBy\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"searchTerm\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"where\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"fields\",\n    \"pageSize\",\n    \"sortBy\",\n    \"searchTerm\",\n    \"where\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetListViewRecordsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-list-view-records-request-schema.json
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
title: GetListViewRecordsRequest
---
