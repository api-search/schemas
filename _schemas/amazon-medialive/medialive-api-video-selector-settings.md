---
description: Video Selector Settings
layout: schema
name: VideoSelectorSettings
properties_list:
- description: ''
  name: VideoSelectorPid
  type: object
- description: ''
  name: VideoSelectorProgramId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-video-selector-settings-schema.json
slug: medialive-api-video-selector-settings
source_filename: medialive-api-video-selector-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-selector-settings-schema.json\",\n  \"title\": \"VideoSelectorSettings\",\n  \"description\": \"Video Selector Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VideoSelectorPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoSelectorPid\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoSelectorPid\"\n          }\n        }\n      ]\n    },\n    \"VideoSelectorProgramId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoSelectorProgramId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoSelectorProgramId\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-selector-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: VideoSelectorSettings
---
