---
description: Clip range configuration for the VOD source associated with the program.
layout: schema
name: ClipRange
properties_list:
- description: ''
  name: EndOffsetMillis
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-clip-range-schema.json
slug: mediatailor-api-clip-range
source_filename: mediatailor-api-clip-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-clip-range-schema.json\",\n  \"title\": \"ClipRange\",\n  \"description\": \"Clip range configuration for the VOD source associated with the program.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndOffsetMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The end offset of the clip range, in milliseconds, starting from the beginning of the VOD source associated with the program.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndOffsetMillis\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-clip-range-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ClipRange
---
