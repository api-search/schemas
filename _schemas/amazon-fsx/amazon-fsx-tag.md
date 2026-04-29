---
description: A key-value metadata label applied to an Amazon FSx resource.
layout: schema
name: Tag
properties_list:
- description: Tag key.
  name: Key
  type: string
- description: Tag value.
  name: Value
  type: string
provider_name: Amazon FSx
provider_slug: amazon-fsx
schema_file: json-schema/amazon-fsx-tag-schema.json
slug: amazon-fsx-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A key-value metadata label applied to an Amazon FSx resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"Tag key.\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"Tag value.\"\n    }\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-tag-schema.json
tags:
- AWS
- File Systems
- Lustre
- NetApp
- OpenZFS
- Storage
- Windows
title: Tag
---
