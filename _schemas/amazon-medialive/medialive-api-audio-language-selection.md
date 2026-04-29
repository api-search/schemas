---
description: Audio Language Selection
layout: schema
name: AudioLanguageSelection
properties_list:
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: LanguageSelectionPolicy
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-language-selection-schema.json
slug: medialive-api-audio-language-selection
source_filename: medialive-api-audio-language-selection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-language-selection-schema.json\",\n  \"title\": \"AudioLanguageSelection\",\n  \"description\": \"Audio Language Selection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageCode\"\n          },\n          \"description\": \"Selects a specific three-letter language code from within an audio source.\"\n        }\n      ]\n    },\n    \"LanguageSelectionPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioLanguageSelectionPolicy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageSelectionPolicy\"\n          },\n          \"description\"\
  : \"When set to \\\"strict\\\", the transport stream demux strictly identifies audio streams by their language descriptor. If a PMT update occurs such that an audio stream matching the initially selected language is no longer present then mute will be encoded until the language returns. If \\\"loose\\\", then on a PMT update the demux will choose another audio stream in the program with the same stream type if it can't find one with the same language.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LanguageCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-language-selection-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioLanguageSelection
---
