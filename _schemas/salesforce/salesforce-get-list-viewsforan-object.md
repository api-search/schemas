---
description: ''
layout: schema
name: GetListViewsforanObject
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: currentPageToken
  type: string
- description: ''
  name: currentPageUrl
  type: string
- description: ''
  name: lists
  type: array
- description: ''
  name: nextPageToken
  type: '[''string'', ''null'']'
- description: ''
  name: nextPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: objectApiName
  type: string
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: previousPageToken
  type: '[''string'', ''null'']'
- description: ''
  name: previousPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: queryString
  type: '[''string'', ''null'']'
- description: ''
  name: recentListsOnly
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-list-viewsforan-object-schema.json
slug: salesforce-get-list-viewsforan-object
source_filename: salesforce-get-list-viewsforan-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"currentPageToken\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"currentPageUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"lists\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"apiName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          }\n     \
  \   },\n        \"required\": [\n          \"apiName\",\n          \"id\",\n          \"label\",\n          \"url\"\n        ]\n      }\n    },\n    \"nextPageToken\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"CAUQAA\"\n    },\n    \"nextPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"objectApiName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"previousPageToken\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"CAUQAA\"\n    },\n    \"previousPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"queryString\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"recentListsOnly\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"\
  required\": [\n    \"count\",\n    \"currentPageToken\",\n    \"currentPageUrl\",\n    \"lists\",\n    \"nextPageToken\",\n    \"nextPageUrl\",\n    \"objectApiName\",\n    \"pageSize\",\n    \"previousPageToken\",\n    \"previousPageUrl\",\n    \"queryString\",\n    \"recentListsOnly\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetListViewsforanObject\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-list-viewsforan-object-schema.json
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
title: GetListViewsforanObject
---
