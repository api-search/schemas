---
description: Request body for the Apache Druid SQL query API (POST /druid/v2/sql).
layout: schema
name: SqlQueryRequest
properties_list:
- description: SQL query string to execute.
  name: query
  type: string
- description: Format for the query results.
  name: resultFormat
  type: string
- description: Whether to return column names in the first row (for array/objectLines formats).
  name: header
  type: boolean
- description: Whether to include column data types in a header row.
  name: typesHeader
  type: boolean
- description: Whether to include SQL type names in a header row.
  name: sqlTypesHeader
  type: boolean
- description: Query context parameters for controlling execution behavior.
  name: context
  type: object
- description: Parameterized query values.
  name: parameters
  type: array
provider_name: Apache Druid
provider_slug: apache-druid
schema_file: json-schema/apache-druid-sql-query-request-schema.json
slug: apache-druid-sql-query-request
source_filename: apache-druid-sql-query-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-druid/refs/heads/main/json-schema/apache-druid-sql-query-request-schema.json\",\n  \"title\": \"SqlQueryRequest\",\n  \"description\": \"Request body for the Apache Druid SQL query API (POST /druid/v2/sql).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"SQL query string to execute.\",\n      \"example\": \"SELECT __time, page, added FROM wikipedia WHERE __time > '2015-09-12' LIMIT 10\"\n    },\n    \"resultFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Format for the query results.\",\n      \"enum\": [\n        \"object\",\n        \"array\",\n        \"objectLines\",\n        \"arrayLines\",\n        \"csv\"\n      ],\n      \"default\": \"object\",\n      \"example\": \"object\"\n    },\n    \"header\": {\n      \"type\": \"boolean\",\n     \
  \ \"description\": \"Whether to return column names in the first row (for array/objectLines formats).\",\n      \"default\": false,\n      \"example\": false\n    },\n    \"typesHeader\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include column data types in a header row.\",\n      \"default\": false,\n      \"example\": false\n    },\n    \"sqlTypesHeader\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include SQL type names in a header row.\",\n      \"default\": false,\n      \"example\": false\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Query context parameters for controlling execution behavior.\",\n      \"properties\": {\n        \"timeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Query timeout in milliseconds.\",\n          \"example\": 30000\n        },\n        \"priority\": {\n          \"type\": \"integer\",\n          \"description\": \"Query priority (lower\
  \ is higher priority).\",\n          \"example\": 0\n        },\n        \"queryId\": {\n          \"type\": \"string\",\n          \"description\": \"Custom query ID for tracking.\",\n          \"example\": \"my-query-001\"\n        }\n      }\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Parameterized query values.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"VARCHAR\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"example\": \"en\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"query\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-druid/refs/heads/main/json-schema/apache-druid-sql-query-request-schema.json
tags:
- Analytics
- Apache
- Database
- Kafka
- OLAP
- Open Source
- Real-Time
- SQL
- Time Series
title: SqlQueryRequest
---
