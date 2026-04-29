---
description: Collection of list views for an object
layout: schema
name: ListViewCollection
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: currentPageToken
  type: string
- description: ''
  name: nextPageToken
  type: string
- description: ''
  name: previousPageToken
  type: string
- description: ''
  name: results
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-ui-list-view-collection-schema.json
slug: salesforce-ui-list-view-collection
source_filename: salesforce-ui-list-view-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Collection of list views for an object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"currentPageToken\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"previousPageToken\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Summary information about a list view\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"apiName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n  \
  \          \"example\": \"Example Title\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListViewCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-ui-list-view-collection-schema.json
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
title: ListViewCollection
---
