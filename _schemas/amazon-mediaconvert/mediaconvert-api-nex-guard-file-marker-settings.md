---
description: For forensic video watermarking, MediaConvert supports Nagra NexGuard File Marker watermarking. MediaConvert supports both PreRelease Content (NGPR/G2) and OTT Streaming workflows.
layout: schema
name: NexGuardFileMarkerSettings
properties_list:
- description: ''
  name: License
  type: object
- description: ''
  name: Payload
  type: object
- description: ''
  name: Preset
  type: object
- description: ''
  name: Strength
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-nex-guard-file-marker-settings-schema.json
slug: mediaconvert-api-nex-guard-file-marker-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nex-guard-file-marker-settings-schema.json\",\n  \"title\": \"NexGuardFileMarkerSettings\",\n  \"description\": \"For forensic video watermarking, MediaConvert supports Nagra NexGuard File Marker watermarking. MediaConvert supports both PreRelease Content (NGPR/G2) and OTT Streaming workflows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"License\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max100000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"license\"\n          },\n          \"description\": \"Use the base64 license string that Nagra provides you. Enter it directly in your JSON job specification or in the console. Required when you include Nagra NexGuard File Marker watermarking (NexGuardWatermarkingSettings)\
  \ in your job.\"\n        }\n      ]\n    },\n    \"Payload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max4194303\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"payload\"\n          },\n          \"description\": \"Specify the payload ID that you want associated with this output. Valid values vary depending on your Nagra NexGuard forensic watermarking workflow. Required when you include Nagra NexGuard File Marker watermarking (NexGuardWatermarkingSettings) in your job. For PreRelease Content (NGPR/G2), specify an integer from 1 through 4,194,303. You must generate a unique ID for each asset you watermark, and keep a record of which ID you have assigned to each asset. Neither Nagra nor MediaConvert keep track of the relationship between output files and your IDs. For OTT Streaming, create two adaptive bitrate (ABR) stacks for each asset. Do this by setting up two output groups. For one output group, set the value\
  \ of Payload ID (payload) to 0 in every output. For the other output group, set Payload ID (payload) to 1 in every output.\"\n        }\n      ]\n    },\n    \"Preset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max256\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"preset\"\n          },\n          \"description\": \"Enter one of the watermarking preset strings that Nagra provides you. Required when you include Nagra NexGuard File Marker watermarking (NexGuardWatermarkingSettings) in your job.\"\n        }\n      ]\n    },\n    \"Strength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WatermarkingStrength\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"strength\"\n          },\n          \"description\": \"Optional. Ignore this setting unless Nagra support directs you to specify a value. When you don't specify a value here, the Nagra NexGuard library uses its\
  \ default value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nex-guard-file-marker-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NexGuardFileMarkerSettings
---
