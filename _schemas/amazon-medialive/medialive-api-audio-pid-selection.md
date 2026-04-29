---
description: Audio Pid Selection
layout: schema
name: AudioPidSelection
properties_list:
- description: ''
  name: Pid
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-pid-selection-schema.json
slug: medialive-api-audio-pid-selection
source_filename: medialive-api-audio-pid-selection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-pid-selection-schema.json\",\n  \"title\": \"AudioPidSelection\",\n  \"description\": \"Audio Pid Selection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max8191\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pid\"\n          },\n          \"description\": \"Selects a specific PID from within a source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Pid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-pid-selection-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioPidSelection
---
