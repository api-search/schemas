---
description: Video Selector Color Space Settings
layout: schema
name: VideoSelectorColorSpaceSettings
properties_list:
- description: ''
  name: Hdr10Settings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-video-selector-color-space-settings-schema.json
slug: medialive-api-video-selector-color-space-settings
source_filename: medialive-api-video-selector-color-space-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-selector-color-space-settings-schema.json\",\n  \"title\": \"VideoSelectorColorSpaceSettings\",\n  \"description\": \"Video Selector Color Space Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Hdr10Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Hdr10Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hdr10Settings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-selector-color-space-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: VideoSelectorColorSpaceSettings
---
