---
description: ''
layout: schema
name: UpdateaBatchofFavoritesRequest
properties_list:
- description: ''
  name: favorites
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-updatea-batchof-favorites-request-schema.json
slug: salesforce-updatea-batchof-favorites-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"favorites\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"name\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"favorites\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateaBatchofFavoritesRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-updatea-batchof-favorites-request-schema.json
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
title: UpdateaBatchofFavoritesRequest
---
