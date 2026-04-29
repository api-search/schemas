---
description: Rest representation of sql query.
layout: schema
name: SqlQuery
properties_list:
- description: Sql query ID.
  name: id
  type: string
- description: Initiator node.
  name: node
  type: string
- description: Phase.
  name: phase
  type: string
- description: Type.
  name: type
  type: string
- description: Schema.
  name: schema
  type: string
- description: SQL statement.
  name: sql
  type: string
- description: Start time.
  name: startTime
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-sql-query-schema.json
slug: rest-api-sql-query
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-sql-query-schema.json\",\n  \"title\": \"SqlQuery\",\n  \"description\": \"Rest representation of sql query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Sql query ID.\",\n      \"format\": \"uuid\"\n    },\n    \"node\": {\n      \"type\": \"string\",\n      \"description\": \"Initiator node.\"\n    },\n    \"phase\": {\n      \"type\": \"string\",\n      \"description\": \"Phase.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type.\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"Schema.\"\n    },\n    \"sql\": {\n      \"type\": \"string\",\n      \"description\": \"SQL statement.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Start time.\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node\",\n    \"phase\",\n    \"schema\",\n    \"sql\",\n    \"startTime\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-sql-query-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: SqlQuery
---
