---
description: Query execution result.
layout: schema
name: QueryResult
properties_list:
- description: Unique query identifier.
  name: queryId
  type: string
- description: Query execution status.
  name: status
  type: string
- description: Number of rows returned.
  name: rowCount
  type: integer
- description: Column metadata.
  name: columns
  type: array
- description: Result rows.
  name: rows
  type: array
- description: Error message if query failed.
  name: errorMessage
  type: string
provider_name: Teradata
provider_slug: teradata
schema_file: json-schema/query-service-api-query-result-schema.json
slug: query-service-api-query-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/query-service-api-query-result-schema.json\",\n  \"title\": \"QueryResult\",\n  \"description\": \"Query execution result.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queryId\": { \"type\": \"string\", \"description\": \"Unique query identifier.\" },\n    \"status\": { \"type\": \"string\", \"description\": \"Query execution status.\", \"enum\": [\"running\", \"completed\", \"failed\", \"cancelled\"] },\n    \"rowCount\": { \"type\": \"integer\", \"description\": \"Number of rows returned.\" },\n    \"columns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\", \"description\": \"Column name.\" },\n          \"type\": { \"type\": \"string\", \"description\": \"Column data type.\" }\n        }\n \
  \     },\n      \"description\": \"Column metadata.\"\n    },\n    \"rows\": { \"type\": \"array\", \"items\": { \"type\": \"array\", \"items\": {} }, \"description\": \"Result rows.\" },\n    \"errorMessage\": { \"type\": \"string\", \"description\": \"Error message if query failed.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/query-service-api-query-result-schema.json
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
title: QueryResult
---
