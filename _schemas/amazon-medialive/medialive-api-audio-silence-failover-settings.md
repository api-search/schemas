---
description: Placeholder documentation for AudioSilenceFailoverSettings
layout: schema
name: AudioSilenceFailoverSettings
properties_list:
- description: ''
  name: AudioSelectorName
  type: object
- description: ''
  name: AudioSilenceThresholdMsec
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-silence-failover-settings-schema.json
slug: medialive-api-audio-silence-failover-settings
source_filename: medialive-api-audio-silence-failover-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-silence-failover-settings-schema.json\",\n  \"title\": \"AudioSilenceFailoverSettings\",\n  \"description\": \"Placeholder documentation for AudioSilenceFailoverSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioSelectorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioSelectorName\"\n          },\n          \"description\": \"The name of the audio selector in the input that MediaLive should monitor to detect silence. Select your most important rendition. If you didn't create an audio selector in this input, leave blank.\"\n        }\n      ]\n    },\n    \"AudioSilenceThresholdMsec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"audioSilenceThresholdMsec\"\n          },\n          \"description\": \"The amount of time (in milliseconds) that the active input must be silent before automatic input failover occurs. Silence is defined as audio loss or audio quieter than -50 dBFS.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AudioSelectorName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-silence-failover-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AudioSilenceFailoverSettings
---
