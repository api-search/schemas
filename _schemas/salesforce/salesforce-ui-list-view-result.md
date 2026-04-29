---
description: Data and metadata for a list view
layout: schema
name: ListViewResult
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: records
  type: array
- description: ''
  name: sortBy
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-ui-list-view-result-schema.json
slug: salesforce-ui-list-view-result
source_filename: salesforce-ui-list-view-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Data and metadata for a list view\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"sortBy\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListViewResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-ui-list-view-result-schema.json
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
title: ListViewResult
---
