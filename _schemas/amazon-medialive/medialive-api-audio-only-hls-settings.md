---
description: Audio Only Hls Settings
layout: schema
name: AudioOnlyHlsSettings
properties_list:
- description: ''
  name: AudioGroupId
  type: object
- description: ''
  name: AudioOnlyImage
  type: object
- description: ''
  name: AudioTrackType
  type: object
- description: ''
  name: SegmentType
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-only-hls-settings-schema.json
slug: medialive-api-audio-only-hls-settings
source_filename: medialive-api-audio-only-hls-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-only-hls-settings-schema.json\",\n  \"title\": \"AudioOnlyHlsSettings\",\n  \"description\": \"Audio Only Hls Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioGroupId\"\n          },\n          \"description\": \"Specifies the group to which the audio Rendition belongs.\"\n        }\n      ]\n    },\n    \"AudioOnlyImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLocation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioOnlyImage\"\n          },\n          \"description\": \"Optional. Specifies the .jpg or .png image to use\
  \ as the cover art for an audio-only output. We recommend a low bit-size file because the image increases the output audio bandwidth.\\n\\nThe image is attached to the audio as an ID3 tag, frame type APIC, picture type 0x10, as per the \\\"ID3 tag version 2.4.0 - Native Frames\\\" standard.\"\n        }\n      ]\n    },\n    \"AudioTrackType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioOnlyHlsTrackType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioTrackType\"\n          },\n          \"description\": \"Four types of audio-only tracks are supported:\\n\\nAudio-Only Variant Stream\\nThe client can play back this audio-only stream instead of video in low-bandwidth scenarios. Represented as an EXT-X-STREAM-INF in the HLS manifest.\\n\\nAlternate Audio, Auto Select, Default\\nAlternate rendition that the client should try to play back by default. Represented as an EXT-X-MEDIA in the HLS manifest with DEFAULT=YES, AUTOSELECT=YES\\\
  n\\nAlternate Audio, Auto Select, Not Default\\nAlternate rendition that the client may try to play back by default. Represented as an EXT-X-MEDIA in the HLS manifest with DEFAULT=NO, AUTOSELECT=YES\\n\\nAlternate Audio, not Auto Select\\nAlternate rendition that the client will not try to play back by default. Represented as an EXT-X-MEDIA in the HLS manifest with DEFAULT=NO, AUTOSELECT=NO\"\n        }\n      ]\n    },\n    \"SegmentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioOnlyHlsSegmentType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentType\"\n          },\n          \"description\": \"Specifies the segment type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-only-hls-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioOnlyHlsSettings
---
