---
description: The <code>CreatePresetResponse</code> structure.
layout: schema
name: CreatePresetResponse
properties_list:
- description: ''
  name: Preset
  type: object
- description: ''
  name: Warning
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-create-preset-response-schema.json
slug: amazon-elastic-transcoder-create-preset-response
source_filename: amazon-elastic-transcoder-create-preset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-create-preset-response-schema.json\",\n  \"title\": \"CreatePresetResponse\",\n  \"description\": \"The <code>CreatePresetResponse</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Preset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Preset\"\n        },\n        {\n          \"description\": \"A section of the response body that provides information about the preset that is created.\"\n        }\n      ]\n    },\n    \"Warning\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"If the preset settings don't comply with the standards for the video codec but Elastic Transcoder created the preset, this message explains the reason\
  \ the preset settings don't meet the standard. Elastic Transcoder created the preset because the settings might produce acceptable output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-create-preset-response-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: CreatePresetResponse
---
