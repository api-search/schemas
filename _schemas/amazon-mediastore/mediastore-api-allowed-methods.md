---
description: AllowedMethods schema from Amazon MediaStore API
layout: schema
name: AllowedMethods
properties_list: []
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-allowed-methods-schema.json
slug: mediastore-api-allowed-methods
source_filename: mediastore-api-allowed-methods-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-allowed-methods-schema.json\",\n  \"title\": \"AllowedMethods\",\n  \"description\": \"AllowedMethods schema from Amazon MediaStore API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/MethodName\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 4\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-allowed-methods-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AllowedMethods
---
