---
description: A file on a snowflake stage.
layout: schema
name: StageFile
properties_list:
- description: Name of the file.
  name: name
  type: string
- description: Size of the file.
  name: size
  type: string
- description: md5 hash of the file.
  name: md5
  type: string
- description: Date and time when the file was last modified.
  name: last_modified
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stage-stage-file-schema.json
slug: stage-stage-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StageFile\",\n  \"type\": \"object\",\n  \"description\": \"A file on a snowflake stage.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the file.\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"Size of the file.\"\n    },\n    \"md5\": {\n      \"type\": \"string\",\n      \"description\": \"md5 hash of the file.\"\n    },\n    \"last_modified\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the file was last modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stage-stage-file-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StageFile
---
