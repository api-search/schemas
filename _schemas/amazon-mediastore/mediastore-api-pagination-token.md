---
description: PaginationToken schema from Amazon MediaStore API
layout: schema
name: PaginationToken
properties_list: []
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-pagination-token-schema.json
slug: mediastore-api-pagination-token
source_filename: mediastore-api-pagination-token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-pagination-token-schema.json\",\n  \"title\": \"PaginationToken\",\n  \"description\": \"PaginationToken schema from Amazon MediaStore API\",\n  \"type\": \"string\",\n  \"pattern\": \"[0-9A-Za-z=/+]+\",\n  \"minLength\": 1,\n  \"maxLength\": 1024\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-pagination-token-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: PaginationToken
---
