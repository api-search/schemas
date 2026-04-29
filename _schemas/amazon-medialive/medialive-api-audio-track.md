---
description: Audio Track
layout: schema
name: AudioTrack
properties_list:
- description: ''
  name: Track
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-track-schema.json
slug: medialive-api-audio-track
source_filename: medialive-api-audio-track-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-track-schema.json\",\n  \"title\": \"AudioTrack\",\n  \"description\": \"Audio Track\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Track\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"track\"\n          },\n          \"description\": \"1-based integer value that maps to a specific audio track\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Track\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-track-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioTrack
---
