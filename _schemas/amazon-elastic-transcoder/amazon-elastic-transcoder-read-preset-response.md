---
description: The <code>ReadPresetResponse</code> structure.
layout: schema
name: ReadPresetResponse
properties_list:
- description: ''
  name: Preset
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-read-preset-response-schema.json
slug: amazon-elastic-transcoder-read-preset-response
source_filename: amazon-elastic-transcoder-read-preset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-read-preset-response-schema.json\",\n  \"title\": \"ReadPresetResponse\",\n  \"description\": \"The <code>ReadPresetResponse</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Preset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Preset\"\n        },\n        {\n          \"description\": \"A section of the response body that provides information about the preset.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-read-preset-response-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: ReadPresetResponse
---
