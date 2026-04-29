---
description: TagKey schema from Amazon MediaStore API
layout: schema
name: TagKey
properties_list: []
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-tag-key-schema.json
slug: mediastore-api-tag-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-tag-key-schema.json\",\n  \"title\": \"TagKey\",\n  \"description\": \"TagKey schema from Amazon MediaStore API\",\n  \"type\": \"string\",\n  \"pattern\": \"[\\\\p{L}\\\\p{Z}\\\\p{N}_.:/=+\\\\-@]*\",\n  \"minLength\": 1,\n  \"maxLength\": 128\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-tag-key-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TagKey
---
