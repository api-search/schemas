---
description: Collection of records matching a lookup search
layout: schema
name: LookupRecordsCollection
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: lookupResults
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-ui-lookup-records-collection-schema.json
slug: salesforce-ui-lookup-records-collection
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Collection of records matching a lookup search\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"lookupResults\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayValue\": {\n            \"type\": \"string\"\n          },\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LookupRecordsCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-ui-lookup-records-collection-schema.json
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
title: LookupRecordsCollection
---
