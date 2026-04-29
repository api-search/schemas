---
description: SqlQueryResponse schema from Apache Pinot
layout: schema
name: SqlQueryResponse
properties_list:
- description: ''
  name: resultTable
  type: object
- description: ''
  name: numDocsScanned
  type: integer
- description: ''
  name: totalDocs
  type: integer
- description: ''
  name: timeUsedMs
  type: integer
- description: ''
  name: numServersQueried
  type: integer
- description: ''
  name: numServersResponded
  type: integer
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-sql-query-response-schema.json
slug: apache-pinot-sql-query-response
source_filename: apache-pinot-sql-query-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-sql-query-response-schema.json\",\n  \"title\": \"SqlQueryResponse\",\n  \"description\": \"SqlQueryResponse schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resultTable\": {\n      \"$ref\": \"#/components/schemas/ResultTable\"\n    },\n    \"numDocsScanned\": {\n      \"type\": \"integer\",\n      \"example\": 1000\n    },\n    \"totalDocs\": {\n      \"type\": \"integer\",\n      \"example\": 10000\n    },\n    \"timeUsedMs\": {\n      \"type\": \"integer\",\n      \"example\": 45\n    },\n    \"numServersQueried\": {\n      \"type\": \"integer\",\n      \"example\": 4\n    },\n    \"numServersResponded\": {\n      \"type\": \"integer\",\n      \"example\": 4\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-sql-query-response-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: SqlQueryResponse
---
