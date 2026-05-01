---
description: Use Manual audio remixing (RemixSettings) to adjust audio levels for each audio channel in each output of your job. With audio remixing, you can output more or fewer audio channels than your input audio source provides.
layout: schema
name: RemixSettings
properties_list:
- description: ''
  name: ChannelMapping
  type: object
- description: ''
  name: ChannelsIn
  type: object
- description: ''
  name: ChannelsOut
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-remix-settings-schema.json
slug: mediaconvert-api-remix-settings
source_filename: mediaconvert-api-remix-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-remix-settings-schema.json\",\n  \"title\": \"RemixSettings\",\n  \"description\": \"Use Manual audio remixing (RemixSettings) to adjust audio levels for each audio channel in each output of your job. With audio remixing, you can output more or fewer audio channels than your input audio source provides.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelMapping\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelMapping\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelMapping\"\n          },\n          \"description\": \"Channel mapping (ChannelMapping) contains the group of fields that hold the remixing value for each channel, in dB. Specify remix values to indicate how much of the content from your input\
  \ audio channel you want in your output audio channels. Each instance of the InputChannels or InputChannelsFineTune array specifies these values for one output channel. Use one instance of this array for each output channel. In the console, each array corresponds to a column in the graphical depiction of the mapping matrix. The rows of the graphical matrix correspond to input channels. Valid values are within the range from -60 (mute) through 6. A setting of 0 passes the input channel unchanged to the output channel (no attenuation or amplification). Use InputChannels or InputChannelsFineTune to specify your remix values. Don't use both.\"\n        }\n      ]\n    },\n    \"ChannelsIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max64\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelsIn\"\n          },\n          \"description\": \"Specify the number of audio channels from your input that you want to use in your\
  \ output. With remixing, you might combine or split the data in these channels, so the number of channels in your final output might be different. If you are doing both input channel mapping and output channel mapping, the number of output channels in your input mapping must be the same as the number of input channels in your output mapping.\"\n        }\n      ]\n    },\n    \"ChannelsOut\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max64\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelsOut\"\n          },\n          \"description\": \"Specify the number of channels in this output after remixing. Valid values: 1, 2, 4, 6, 8... 64. (1 and even numbers to 64.) If you are doing both input channel mapping and output channel mapping, the number of output channels in your input mapping must be the same as the number of input channels in your output mapping.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-remix-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: RemixSettings
---
