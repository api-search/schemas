---
description: You can add a tag for this mono-channel audio track to mimic its placement in a multi-channel layout. For example, if this track is the left surround channel, choose Left surround (LS).
layout: schema
name: AudioChannelTag
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-audio-channel-tag-schema.json
slug: mediaconvert-api-audio-channel-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-channel-tag-schema.json\",\n  \"title\": \"AudioChannelTag\",\n  \"description\": \"You can add a tag for this mono-channel audio track to mimic its placement in a multi-channel layout. For example, if this track is the left surround channel, choose Left surround (LS).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"L\",\n    \"R\",\n    \"C\",\n    \"LFE\",\n    \"LS\",\n    \"RS\",\n    \"LC\",\n    \"RC\",\n    \"CS\",\n    \"LSD\",\n    \"RSD\",\n    \"TCS\",\n    \"VHL\",\n    \"VHC\",\n    \"VHR\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-channel-tag-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioChannelTag
---
