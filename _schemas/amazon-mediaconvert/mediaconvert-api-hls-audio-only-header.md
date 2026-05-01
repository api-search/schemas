---
description: Ignore this setting unless you are using FairPlay DRM with Verimatrix and you encounter playback issues. Keep the default value, Include (INCLUDE), to output audio-only headers. Choose Exclude (EXCLUDE) to remove the audio-only headers from your audio segments.
layout: schema
name: HlsAudioOnlyHeader
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-audio-only-header-schema.json
slug: mediaconvert-api-hls-audio-only-header
source_filename: mediaconvert-api-hls-audio-only-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-audio-only-header-schema.json\",\n  \"title\": \"HlsAudioOnlyHeader\",\n  \"description\": \"Ignore this setting unless you are using FairPlay DRM with Verimatrix and you encounter playback issues. Keep the default value, Include (INCLUDE), to output audio-only headers. Choose Exclude (EXCLUDE) to remove the audio-only headers from your audio segments.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"INCLUDE\",\n    \"EXCLUDE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-audio-only-header-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsAudioOnlyHeader
---
