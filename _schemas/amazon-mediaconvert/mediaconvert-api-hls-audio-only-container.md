---
description: Use this setting only in audio-only outputs. Choose MPEG-2 Transport Stream (M2TS) to create a file in an MPEG2-TS container. Keep the default value Automatic (AUTOMATIC) to create a raw audio-only file with no container. Regardless of the value that you specify here, if this output has video, the service will place outputs into an MPEG2-TS container.
layout: schema
name: HlsAudioOnlyContainer
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-audio-only-container-schema.json
slug: mediaconvert-api-hls-audio-only-container
source_filename: mediaconvert-api-hls-audio-only-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-audio-only-container-schema.json\",\n  \"title\": \"HlsAudioOnlyContainer\",\n  \"description\": \"Use this setting only in audio-only outputs. Choose MPEG-2 Transport Stream (M2TS) to create a file in an MPEG2-TS container. Keep the default value Automatic (AUTOMATIC) to create a raw audio-only file with no container. Regardless of the value that you specify here, if this output has video, the service will place outputs into an MPEG2-TS container.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AUTOMATIC\",\n    \"M2TS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-audio-only-container-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsAudioOnlyContainer
---
