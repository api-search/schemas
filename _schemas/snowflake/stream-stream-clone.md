---
description: ''
layout: schema
name: StreamClone
properties_list:
- description: Name of the stream
  name: name
  type: string
- description: user comment associated to an object in the dictionary
  name: comment
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stream-stream-clone-schema.json
slug: stream-stream-clone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StreamClone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the stream\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"user comment associated to an object in the dictionary\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stream-stream-clone-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StreamClone
---
