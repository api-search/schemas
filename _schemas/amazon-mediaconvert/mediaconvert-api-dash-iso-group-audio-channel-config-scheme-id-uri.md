---
description: 'Use this setting only when your audio codec is a Dolby one (AC3, EAC3, or Atmos) and your downstream workflow requires that your DASH manifest use the Dolby channel configuration tag, rather than the MPEG one. For example, you might need to use this to make dynamic ad insertion work. Specify which audio channel configuration scheme ID URI MediaConvert writes in your DASH manifest. Keep the default value, MPEG channel configuration (MPEG_CHANNEL_CONFIGURATION), to have MediaConvert write this: urn:mpeg:mpegB:cicp:ChannelConfiguration. Choose Dolby channel configuration (DOLBY_CHANNEL_CONFIGURATION) to have MediaConvert write this instead: tag:dolby.com,2014:dash:audio_channel_configuration:2011.'
layout: schema
name: DashIsoGroupAudioChannelConfigSchemeIdUri
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dash-iso-group-audio-channel-config-scheme-id-uri-schema.json
slug: mediaconvert-api-dash-iso-group-audio-channel-config-scheme-id-uri
source_filename: mediaconvert-api-dash-iso-group-audio-channel-config-scheme-id-uri-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-group-audio-channel-config-scheme-id-uri-schema.json\",\n  \"title\": \"DashIsoGroupAudioChannelConfigSchemeIdUri\",\n  \"description\": \"Use this setting only when your audio codec is a Dolby one (AC3, EAC3, or Atmos) and your downstream workflow requires that your DASH manifest use the Dolby channel configuration tag, rather than the MPEG one. For example, you might need to use this to make dynamic ad insertion work. Specify which audio channel configuration scheme ID URI MediaConvert writes in your DASH manifest. Keep the default value, MPEG channel configuration (MPEG_CHANNEL_CONFIGURATION), to have MediaConvert write this: urn:mpeg:mpegB:cicp:ChannelConfiguration. Choose Dolby channel configuration (DOLBY_CHANNEL_CONFIGURATION) to have MediaConvert write this instead:\
  \ tag:dolby.com,2014:dash:audio_channel_configuration:2011.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"MPEG_CHANNEL_CONFIGURATION\",\n    \"DOLBY_CHANNEL_CONFIGURATION\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-group-audio-channel-config-scheme-id-uri-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DashIsoGroupAudioChannelConfigSchemeIdUri
---
