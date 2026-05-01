---
description: Audio Selector Settings
layout: schema
name: AudioSelectorSettings
properties_list:
- description: ''
  name: AudioHlsRenditionSelection
  type: object
- description: ''
  name: AudioLanguageSelection
  type: object
- description: ''
  name: AudioPidSelection
  type: object
- description: ''
  name: AudioTrackSelection
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-selector-settings-schema.json
slug: medialive-api-audio-selector-settings
source_filename: medialive-api-audio-selector-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-selector-settings-schema.json\",\n  \"title\": \"AudioSelectorSettings\",\n  \"description\": \"Audio Selector Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioHlsRenditionSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioHlsRenditionSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioHlsRenditionSelection\"\n          }\n        }\n      ]\n    },\n    \"AudioLanguageSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioLanguageSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioLanguageSelection\"\n          }\n        }\n      ]\n    },\n    \"AudioPidSelection\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/AudioPidSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioPidSelection\"\n          }\n        }\n      ]\n    },\n    \"AudioTrackSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioTrackSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioTrackSelection\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-selector-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AudioSelectorSettings
---
