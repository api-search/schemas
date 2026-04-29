---
description: SQL query request
layout: schema
name: QueryRequest
properties_list:
- description: SQL query to execute
  name: sql
  type: string
- description: Project name to query
  name: project
  type: string
- description: Result offset for pagination
  name: offset
  type: integer
- description: Maximum number of results
  name: limit
  type: integer
- description: Accept partial results if query times out
  name: acceptPartial
  type: boolean
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-query-request-schema.json
slug: rest-api-query-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-query-request-schema.json\",\n  \"title\": \"QueryRequest\",\n  \"description\": \"SQL query request\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sql\": {\n      \"type\": \"string\",\n      \"description\": \"SQL query to execute\",\n      \"example\": \"SELECT count(*) FROM kylin_sales\"\n    },\n    \"project\": {\n      \"type\": \"string\",\n      \"description\": \"Project name to query\",\n      \"example\": \"learn_kylin\"\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Result offset for pagination\",\n      \"example\": 0\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results\",\n      \"example\": 50000\n    },\n    \"acceptPartial\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Accept partial results if query times out\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"sql\",\n    \"project\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-query-request-schema.json
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: QueryRequest
---
