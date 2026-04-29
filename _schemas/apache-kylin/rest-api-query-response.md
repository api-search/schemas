---
description: SQL query response
layout: schema
name: QueryResponse
properties_list:
- description: Result column metadata
  name: columnMetas
  type: array
- description: Query result rows
  name: results
  type: array
- description: ''
  name: queryId
  type: string
- description: ''
  name: isException
  type: boolean
- description: ''
  name: exceptionMessage
  type: string
- description: Query duration in milliseconds
  name: duration
  type: integer
- description: ''
  name: totalScanCount
  type: integer
- description: ''
  name: totalScanBytes
  type: integer
- description: ''
  name: hitExceptionCache
  type: boolean
- description: ''
  name: storageCacheUsed
  type: boolean
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-query-response-schema.json
slug: rest-api-query-response
source_filename: rest-api-query-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-query-response-schema.json\",\n  \"title\": \"QueryResponse\",\n  \"description\": \"SQL query response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"columnMetas\": {\n      \"type\": \"array\",\n      \"description\": \"Result column metadata\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Query result rows\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"queryId\": {\n      \"type\": \"string\",\n      \"example\": \"query-1234\"\n    },\n    \"isException\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"exceptionMessage\": {\n      \"type\": \"string\"\n    },\n    \"duration\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Query duration in milliseconds\",\n      \"example\": 120\n    },\n    \"totalScanCount\": {\n      \"type\": \"integer\",\n      \"example\": 10000\n    },\n    \"totalScanBytes\": {\n      \"type\": \"integer\",\n      \"example\": 409600\n    },\n    \"hitExceptionCache\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"storageCacheUsed\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-query-response-schema.json
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: QueryResponse
---
