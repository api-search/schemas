---
description: Audio Watermark Settings
layout: schema
name: AudioWatermarkSettings
properties_list:
- description: ''
  name: NielsenWatermarksSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-watermark-settings-schema.json
slug: medialive-api-audio-watermark-settings
source_filename: medialive-api-audio-watermark-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-watermark-settings-schema.json\",\n  \"title\": \"AudioWatermarkSettings\",\n  \"description\": \"Audio Watermark Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NielsenWatermarksSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenWatermarksSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenWatermarksSettings\"\n          },\n          \"description\": \"Settings to configure Nielsen Watermarks in the audio encode\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-watermark-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AudioWatermarkSettings
---
