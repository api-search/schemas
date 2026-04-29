---
description: ''
layout: schema
name: StreamSource
properties_list:
- description: 'Type of the source. Possible values include: stream, table, view'
  name: src_type
  type: string
- description: Name of the source whose changes are tracked by the stream
  name: name
  type: string
- description: Database name to which stream source type belongs. If not provided, database name provided in the path param will be used.
  name: database_name
  type: string
- description: Schema name to which stream source type belongs. If not provided, schema name provided in the path param will be used.
  name: schema_name
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stream-stream-source-schema.json
slug: stream-stream-source
source_filename: stream-stream-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StreamSource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"src_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the source. Possible values include: stream, table, view\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the source whose changes are tracked by the stream\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"Database name to which stream source type belongs. If not provided, database  name provided in the path param will be used.\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"Schema name to which stream source type belongs. If not provided, schema name provided in the path param will be used.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stream-stream-source-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StreamSource
---
