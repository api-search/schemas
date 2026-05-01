---
description: ExposeHeaders schema from Amazon MediaStore API
layout: schema
name: ExposeHeaders
properties_list: []
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-expose-headers-schema.json
slug: mediastore-api-expose-headers
source_filename: mediastore-api-expose-headers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-expose-headers-schema.json\",\n  \"title\": \"ExposeHeaders\",\n  \"description\": \"ExposeHeaders schema from Amazon MediaStore API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Header\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 100\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-expose-headers-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ExposeHeaders
---
