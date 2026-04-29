---
description: When you mimic a multi-channel audio layout with multiple mono-channel tracks, you can tag each channel layout manually. For example, you would tag the tracks that contain your left, right, and center audio with Left (L), Right (R), and Center (C), respectively. When you don't specify a value, MediaConvert labels your track as Center (C) by default. To use audio layout tagging, your output must be in a QuickTime (.mov) container; your audio codec must be AAC, WAV, or AIFF; and you must set up your audio track to have only one channel.
layout: schema
name: AudioChannelTaggingSettings
properties_list:
- description: ''
  name: ChannelTag
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-audio-channel-tagging-settings-schema.json
slug: mediaconvert-api-audio-channel-tagging-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-channel-tagging-settings-schema.json\",\n  \"title\": \"AudioChannelTaggingSettings\",\n  \"description\": \"When you mimic a multi-channel audio layout with multiple mono-channel tracks, you can tag each channel layout manually. For example, you would tag the tracks that contain your left, right, and center audio with Left (L), Right (R), and Center (C), respectively. When you don't specify a value, MediaConvert labels your track as Center (C) by default. To use audio layout tagging, your output must be in a QuickTime (.mov) container; your audio codec must be AAC, WAV, or AIFF; and you must set up your audio track to have only one channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelTag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioChannelTag\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"channelTag\"\n          },\n          \"description\": \"You can add a tag for this mono-channel audio track to mimic its placement in a multi-channel layout. For example, if this track is the left surround channel, choose Left surround (LS).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-channel-tagging-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioChannelTaggingSettings
---
