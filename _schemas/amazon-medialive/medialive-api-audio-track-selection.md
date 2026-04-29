---
description: Audio Track Selection
layout: schema
name: AudioTrackSelection
properties_list:
- description: ''
  name: Tracks
  type: object
- description: ''
  name: DolbyEDecode
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-track-selection-schema.json
slug: medialive-api-audio-track-selection
source_filename: medialive-api-audio-track-selection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-track-selection-schema.json\",\n  \"title\": \"AudioTrackSelection\",\n  \"description\": \"Audio Track Selection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tracks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAudioTrack\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tracks\"\n          },\n          \"description\": \"Selects one or more unique audio tracks from within a source.\"\n        }\n      ]\n    },\n    \"DolbyEDecode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioDolbyEDecode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dolbyEDecode\"\n          },\n          \"description\": \"Configure decoding options for Dolby E streams - these\
  \ should be Dolby E frames carried in PCM streams tagged with SMPTE-337\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Tracks\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-track-selection-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioTrackSelection
---
