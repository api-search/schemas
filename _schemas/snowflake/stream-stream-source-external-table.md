---
description: ''
layout: schema
name: StreamSourceExternalTable
properties_list:
- description: Whether this stream is an insert only stream or not
  name: insert_only
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stream-stream-source-external-table-schema.json
slug: stream-stream-source-external-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StreamSourceExternalTable\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"insert_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this stream is an insert only stream or not\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stream-stream-source-external-table-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StreamSourceExternalTable
---
