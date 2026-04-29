---
description: Specific settings for this type of output.
layout: schema
name: OutputSettings
properties_list:
- description: ''
  name: HlsSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-output-settings-schema.json
slug: mediaconvert-api-output-settings
source_filename: mediaconvert-api-output-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-settings-schema.json\",\n  \"title\": \"OutputSettings\",\n  \"description\": \"Specific settings for this type of output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HlsSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsSettings\"\n          },\n          \"description\": \"Settings for HLS output groups\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OutputSettings
---
