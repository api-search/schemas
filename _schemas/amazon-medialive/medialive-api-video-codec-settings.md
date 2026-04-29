---
description: Video Codec Settings
layout: schema
name: VideoCodecSettings
properties_list:
- description: ''
  name: FrameCaptureSettings
  type: object
- description: ''
  name: H264Settings
  type: object
- description: ''
  name: H265Settings
  type: object
- description: ''
  name: Mpeg2Settings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-video-codec-settings-schema.json
slug: medialive-api-video-codec-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-codec-settings-schema.json\",\n  \"title\": \"VideoCodecSettings\",\n  \"description\": \"Video Codec Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FrameCaptureSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameCaptureSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"frameCaptureSettings\"\n          }\n        }\n      ]\n    },\n    \"H264Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"h264Settings\"\n          }\n        }\n      ]\n    },\n    \"H265Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265Settings\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"h265Settings\"\n          }\n        }\n      ]\n    },\n    \"Mpeg2Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mpeg2Settings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-codec-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VideoCodecSettings
---
