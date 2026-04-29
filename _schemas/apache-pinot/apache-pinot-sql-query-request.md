---
description: SqlQueryRequest schema from Apache Pinot
layout: schema
name: SqlQueryRequest
properties_list:
- description: SQL query to execute
  name: sql
  type: string
- description: Query options key=value pairs
  name: queryOptions
  type: string
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-sql-query-request-schema.json
slug: apache-pinot-sql-query-request
source_filename: apache-pinot-sql-query-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-sql-query-request-schema.json\",\n  \"title\": \"SqlQueryRequest\",\n  \"description\": \"SqlQueryRequest schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sql\": {\n      \"type\": \"string\",\n      \"description\": \"SQL query to execute\",\n      \"example\": \"SELECT COUNT(*) FROM airlineStats WHERE Year = 2014\"\n    },\n    \"queryOptions\": {\n      \"type\": \"string\",\n      \"description\": \"Query options key=value pairs\",\n      \"example\": \"timeoutMs=5000\"\n    }\n  },\n  \"required\": [\n    \"sql\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-sql-query-request-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: SqlQueryRequest
---
