---
description: Channel mapping (ChannelMapping) contains the group of fields that hold the remixing value for each channel, in dB. Specify remix values to indicate how much of the content from your input audio channel you want in your output audio channels. Each instance of the InputChannels or InputChannelsFineTune array specifies these values for one output channel. Use one instance of this array for each output channel. In the console, each array corresponds to a column in the graphical depiction of the mapping matrix. The rows of the graphical matrix correspond to input channels. Valid values are within the range from -60 (mute) through 6. A setting of 0 passes the input channel unchanged to the output channel (no attenuation or amplification). Use InputChannels or InputChannelsFineTune to specify your remix values. Don't use both.
layout: schema
name: ChannelMapping
properties_list:
- description: ''
  name: OutputChannels
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-channel-mapping-schema.json
slug: mediaconvert-api-channel-mapping
source_filename: mediaconvert-api-channel-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-channel-mapping-schema.json\",\n  \"title\": \"ChannelMapping\",\n  \"description\": \"Channel mapping (ChannelMapping) contains the group of fields that hold the remixing value for each channel, in dB. Specify remix values to indicate how much of the content from your input audio channel you want in your output audio channels. Each instance of the InputChannels or InputChannelsFineTune array specifies these values for one output channel. Use one instance of this array for each output channel. In the console, each array corresponds to a column in the graphical depiction of the mapping matrix. The rows of the graphical matrix correspond to input channels. Valid values are within the range from -60 (mute) through 6. A setting of 0 passes the input channel unchanged to the output channel\
  \ (no attenuation or amplification). Use InputChannels or InputChannelsFineTune to specify your remix values. Don't use both.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputChannels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutputChannelMapping\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputChannels\"\n          },\n          \"description\": \"In your JSON job specification, include one child of OutputChannels for each audio channel that you want in your output. Each child should contain one instance of InputChannels or InputChannelsFineTune.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-channel-mapping-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ChannelMapping
---
