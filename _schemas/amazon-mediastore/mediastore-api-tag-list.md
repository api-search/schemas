---
description: TagList schema from Amazon MediaStore API
layout: schema
name: TagList
properties_list: []
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-tag-list-schema.json
slug: mediastore-api-tag-list
source_filename: mediastore-api-tag-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-tag-list-schema.json\",\n  \"title\": \"TagList\",\n  \"description\": \"TagList schema from Amazon MediaStore API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Tag\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 200\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-tag-list-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TagList
---
