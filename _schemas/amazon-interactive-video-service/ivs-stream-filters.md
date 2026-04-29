---
description: Object specifying the stream attribute on which to filter.
layout: schema
name: StreamFilters
properties_list:
- description: ''
  name: health
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-stream-filters-schema.json
slug: ivs-stream-filters
source_filename: ivs-stream-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-filters-schema.json\",\n  \"title\": \"StreamFilters\",\n  \"description\": \"Object specifying the stream attribute on which to filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"health\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamHealth\"\n        },\n        {\n          \"description\": \"The stream\\u2019s health.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-filters-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: StreamFilters
---
