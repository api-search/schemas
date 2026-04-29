---
description: The CORS policy of the container.
layout: schema
name: CorsPolicy
properties_list: []
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-cors-policy-schema.json
slug: mediastore-api-cors-policy
source_filename: mediastore-api-cors-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-cors-policy-schema.json\",\n  \"title\": \"CorsPolicy\",\n  \"description\": \"The CORS policy of the container. \",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/CorsRule\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 100\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-cors-policy-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CorsPolicy
---
