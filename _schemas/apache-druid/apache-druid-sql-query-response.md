---
description: Response from the Apache Druid SQL API with query results and metadata.
layout: schema
name: SqlQueryResponse
properties_list:
- description: Unique ID assigned to this query.
  name: queryId
  type: string
- description: Column names in result order.
  name: columns
  type: array
- description: Column Druid types.
  name: columnTypes
  type: array
- description: Column SQL types.
  name: sqlTypes
  type: array
- description: Query result rows (format depends on resultFormat).
  name: results
  type: array
provider_name: Apache Druid
provider_slug: apache-druid
schema_file: json-schema/apache-druid-sql-query-response-schema.json
slug: apache-druid-sql-query-response
source_filename: apache-druid-sql-query-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-druid/refs/heads/main/json-schema/apache-druid-sql-query-response-schema.json\",\n  \"title\": \"SqlQueryResponse\",\n  \"description\": \"Response from the Apache Druid SQL API with query results and metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queryId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID assigned to this query.\",\n      \"example\": \"abc-123-def-456\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"Column names in result order.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"__time\",\n        \"page\",\n        \"added\"\n      ]\n    },\n    \"columnTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Column Druid types.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n  \
  \    \"example\": [\n        \"TIMESTAMP\",\n        \"STRING\",\n        \"LONG\"\n      ]\n    },\n    \"sqlTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Column SQL types.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"TIMESTAMP\",\n        \"VARCHAR\",\n        \"BIGINT\"\n      ]\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Query result rows (format depends on resultFormat).\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-druid/refs/heads/main/json-schema/apache-druid-sql-query-response-schema.json
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
title: SqlQueryResponse
---
