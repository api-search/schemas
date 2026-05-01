---
description: The <code>ListPresetsResponse</code> structure.
layout: schema
name: ListPresetsResponse
properties_list:
- description: ''
  name: Presets
  type: object
- description: ''
  name: NextPageToken
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-list-presets-response-schema.json
slug: amazon-elastic-transcoder-list-presets-response
source_filename: amazon-elastic-transcoder-list-presets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-list-presets-response-schema.json\",\n  \"title\": \"ListPresetsResponse\",\n  \"description\": \"The <code>ListPresetsResponse</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Presets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Presets\"\n        },\n        {\n          \"description\": \"An array of <code>Preset</code> objects.\"\n        }\n      ]\n    },\n    \"NextPageToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"A value that you use to access the second and subsequent pages of results, if any. When the presets fit on one page or when you've reached the last page of results, the value of <code>NextPageToken</code>\
  \ is <code>null</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-list-presets-response-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: ListPresetsResponse
---
