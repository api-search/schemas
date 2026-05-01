---
description: AllowedOrigins schema from Amazon MediaStore API
layout: schema
name: AllowedOrigins
properties_list: []
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-allowed-origins-schema.json
slug: mediastore-api-allowed-origins
source_filename: mediastore-api-allowed-origins-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-allowed-origins-schema.json\",\n  \"title\": \"AllowedOrigins\",\n  \"description\": \"AllowedOrigins schema from Amazon MediaStore API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Origin\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 100\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-allowed-origins-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AllowedOrigins
---
