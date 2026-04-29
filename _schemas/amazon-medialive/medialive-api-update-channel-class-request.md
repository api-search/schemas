---
description: Channel class that the channel should be updated to.
layout: schema
name: UpdateChannelClassRequest
properties_list:
- description: ''
  name: ChannelClass
  type: object
- description: ''
  name: Destinations
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-update-channel-class-request-schema.json
slug: medialive-api-update-channel-class-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-channel-class-request-schema.json\",\n  \"title\": \"UpdateChannelClassRequest\",\n  \"description\": \"Channel class that the channel should be updated to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelClass\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelClass\"\n          },\n          \"description\": \"The channel class that you wish to update this channel to use.\"\n        }\n      ]\n    },\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutputDestination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinations\"\n          },\n          \"description\"\
  : \"A list of output destinations for this channel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ChannelClass\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-channel-class-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateChannelClassRequest
---
