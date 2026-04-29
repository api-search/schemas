---
description: Audio Selector
layout: schema
name: AudioSelector
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: SelectorSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-selector-schema.json
slug: medialive-api-audio-selector
source_filename: medialive-api-audio-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-selector-schema.json\",\n  \"title\": \"AudioSelector\",\n  \"description\": \"Audio Selector\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of this AudioSelector. AudioDescriptions will use this name to uniquely identify this Selector.  Selector names should be unique per input.\"\n        }\n      ]\n    },\n    \"SelectorSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioSelectorSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"selectorSettings\"\n          },\n         \
  \ \"description\": \"The audio selector settings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-selector-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioSelector
---
