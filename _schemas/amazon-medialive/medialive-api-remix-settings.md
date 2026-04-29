---
description: Remix Settings
layout: schema
name: RemixSettings
properties_list:
- description: ''
  name: ChannelMappings
  type: object
- description: ''
  name: ChannelsIn
  type: object
- description: ''
  name: ChannelsOut
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-remix-settings-schema.json
slug: medialive-api-remix-settings
source_filename: medialive-api-remix-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-remix-settings-schema.json\",\n  \"title\": \"RemixSettings\",\n  \"description\": \"Remix Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAudioChannelMapping\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelMappings\"\n          },\n          \"description\": \"Mapping of input channels to output channels, with appropriate gain adjustments.\"\n        }\n      ]\n    },\n    \"ChannelsIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max16\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelsIn\"\n          },\n          \"description\": \"Number of input channels to\
  \ be used.\"\n        }\n      ]\n    },\n    \"ChannelsOut\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max8\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelsOut\"\n          },\n          \"description\": \"Number of output channels to be produced.\\nValid values: 1, 2, 4, 6, 8\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ChannelMappings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-remix-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: RemixSettings
---
