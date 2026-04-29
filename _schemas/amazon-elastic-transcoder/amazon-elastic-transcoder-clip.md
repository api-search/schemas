---
description: Settings for one clip in a composition. All jobs in a playlist must have the same clip settings.
layout: schema
name: Clip
properties_list:
- description: ''
  name: TimeSpan
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-clip-schema.json
slug: amazon-elastic-transcoder-clip
source_filename: amazon-elastic-transcoder-clip-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-clip-schema.json\",\n  \"title\": \"Clip\",\n  \"description\": \"Settings for one clip in a composition. All jobs in a playlist must have the same clip settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TimeSpan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSpan\"\n        },\n        {\n          \"description\": \"Settings that determine when a clip begins and how long it lasts.\"\n        }\n      ]\n    }\n  },\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-clip-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: Clip
---
