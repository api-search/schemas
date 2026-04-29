---
description: Audio Channel Mapping
layout: schema
name: AudioChannelMapping
properties_list:
- description: ''
  name: InputChannelLevels
  type: object
- description: ''
  name: OutputChannel
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-channel-mapping-schema.json
slug: medialive-api-audio-channel-mapping
source_filename: medialive-api-audio-channel-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-channel-mapping-schema.json\",\n  \"title\": \"AudioChannelMapping\",\n  \"description\": \"Audio Channel Mapping\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputChannelLevels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputChannelLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputChannelLevels\"\n          },\n          \"description\": \"Indices and gain values for each input channel that should be remixed into this output channel.\"\n        }\n      ]\n    },\n    \"OutputChannel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max7\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputChannel\"\n          },\n          \"\
  description\": \"The index of the output channel being produced.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OutputChannel\",\n    \"InputChannelLevels\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-channel-mapping-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioChannelMapping
---
