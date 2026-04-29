---
description: ''
layout: schema
name: LookupTableRequest1
properties_list:
- description: ''
  name: conditions
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-lookup-table-request1-schema.json
slug: salesforce-lookup-table-request1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"conditions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"conditionsList\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"fieldName\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"value\": {\n                \"type\": \"boolean\",\n                \"example\": true\n              }\n            },\n            \"required\": [\n              \"fieldName\",\n              \"value\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"conditionsList\"\n      ]\n    }\n  },\n  \"required\": [\n    \"conditions\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LookupTableRequest1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-lookup-table-request1-schema.json
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
title: LookupTableRequest1
---
