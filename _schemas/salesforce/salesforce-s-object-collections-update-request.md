---
description: ''
layout: schema
name: SObjectCollectionsUpdateRequest
properties_list:
- description: ''
  name: allOrNone
  type: boolean
- description: ''
  name: records
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-s-object-collections-update-request-schema.json
slug: salesforce-s-object-collections-update-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"allOrNone\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"type\"\n            ]\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"NumberOfEmployees\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          }\n        },\n        \"required\": [\n          \"attributes\",\n          \"id\",\n          \"NumberOfEmployees\"\n        ]\n \
  \     }\n    }\n  },\n  \"required\": [\n    \"allOrNone\",\n    \"records\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SObjectCollectionsUpdateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-s-object-collections-update-request-schema.json
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
title: SObjectCollectionsUpdateRequest
---
