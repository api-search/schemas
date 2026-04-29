---
description: The result of a SOQL query, containing the matching records and pagination metadata.
layout: schema
name: QueryResult
properties_list:
- description: The total number of records matching the query. May be larger than the number of records in the current page if the result is paginated.
  name: totalSize
  type: integer
- description: Whether all query results have been returned. If false, use nextRecordsUrl to retrieve the next page.
  name: done
  type: boolean
- description: URL to retrieve the next page of results. Only present when done is false.
  name: nextRecordsUrl
  type: string
- description: Array of SObject records matching the query. May be a partial result if the total exceeds the page size.
  name: records
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-rest-query-result-schema.json
slug: salesforce-rest-query-result
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result of a SOQL query, containing the matching records and pagination metadata.\\n\",\n  \"properties\": {\n    \"totalSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of records matching the query. May be larger than the number of records in the current page if the result is paginated.\\n\",\n      \"example\": 42\n    },\n    \"done\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether all query results have been returned. If false, use nextRecordsUrl to retrieve the next page.\\n\",\n      \"example\": true\n    },\n    \"nextRecordsUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to retrieve the next page of results. Only present when done is false.\\n\",\n      \"format\": \"uri\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"Array of SObject records matching the query.\
  \ May be a partial result if the total exceeds the page size.\\n\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A Salesforce SObject record. Contains an attributes object describing the record type and URL, plus any number of field name/value pairs depending on the object type.\\n\",\n        \"properties\": {\n          \"attributes\": {\n            \"type\": \"object\",\n            \"description\": \"Metadata attributes for this SObject record, including its type and REST API URL.\\n\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"The API name of the SObject type (e.g., Account, Contact).\"\n              },\n              \"url\": {\n                \"type\": \"string\",\n                \"description\": \"The REST API URL for this specific record.\",\n                \"format\": \"uri\"\n  \
  \            }\n            },\n            \"required\": [\n              \"type\"\n            ]\n          },\n          \"Id\": {\n            \"type\": \"string\",\n            \"description\": \"The 18-character globally unique Salesforce record ID.\",\n            \"example\": \"abc123\"\n          }\n        },\n        \"required\": [\n          \"attributes\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"totalSize\",\n    \"done\",\n    \"records\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-rest-query-result-schema.json
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
title: QueryResult
---
