---
description: A tag that can be added to an MemoryDB resource.
layout: schema
name: Tag
properties_list:
- description: The key for the tag.
  name: Key
  type: string
- description: The tag's value.
  name: Value
  type: string
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
schema_file: json-schema/memorydb-api-tag-schema.json
slug: memorydb-api-tag
source_filename: memorydb-api-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A tag that can be added to an MemoryDB resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"description\": \"The key for the tag.\",\n      \"type\": \"string\"\n    },\n    \"Value\": {\n      \"description\": \"The tag's value.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-tag-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Tag
---
