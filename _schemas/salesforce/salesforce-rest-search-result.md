---
description: The result of a SOSL search, containing matching records grouped by SObject type.
layout: schema
name: SearchResult
properties_list:
- description: Array of records matching the SOSL search query. Each record includes the object type in its attributes.
  name: searchRecords
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-rest-search-result-schema.json
slug: salesforce-rest-search-result
source_filename: salesforce-rest-search-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result of a SOSL search, containing matching records grouped by SObject type.\\n\",\n  \"properties\": {\n    \"searchRecords\": {\n      \"type\": \"array\",\n      \"description\": \"Array of records matching the SOSL search query. Each record includes the object type in its attributes.\\n\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A Salesforce SObject record. Contains an attributes object describing the record type and URL, plus any number of field name/value pairs depending on the object type.\\n\",\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"object\",\n            \"description\": \"Metadata attributes for this SObject record, including its type and REST API URL.\\n\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n        \
  \        \"description\": \"The API name of the SObject type (e.g., Account, Contact).\"\n              },\n              \"url\": {\n                \"type\": \"string\",\n                \"description\": \"The REST API URL for this specific record.\",\n                \"format\": \"uri\"\n              }\n            },\n            \"required\": [\n              \"type\"\n            ]\n          },\n          \"Id\": {\n            \"type\": \"string\",\n            \"description\": \"The 18-character globally unique Salesforce record ID.\",\n            \"example\": \"abc123\"\n          }\n        },\n        \"required\": [\n          \"attributes\"\n        ]\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-rest-search-result-schema.json
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
title: SearchResult
---
