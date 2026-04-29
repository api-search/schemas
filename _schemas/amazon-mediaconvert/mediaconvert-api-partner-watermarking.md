---
description: If you work with a third party video watermarking partner, use the group of settings that correspond with your watermarking partner to include watermarks in your output.
layout: schema
name: PartnerWatermarking
properties_list:
- description: ''
  name: NexguardFileMarkerSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-partner-watermarking-schema.json
slug: mediaconvert-api-partner-watermarking
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-partner-watermarking-schema.json\",\n  \"title\": \"PartnerWatermarking\",\n  \"description\": \"If you work with a third party video watermarking partner, use the group of settings that correspond with your watermarking partner to include watermarks in your output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NexguardFileMarkerSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NexGuardFileMarkerSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nexguardFileMarkerSettings\"\n          },\n          \"description\": \"For forensic video watermarking, MediaConvert supports Nagra NexGuard File Marker watermarking. MediaConvert supports both PreRelease Content (NGPR/G2) and OTT Streaming workflows.\"\n     \
  \   }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-partner-watermarking-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PartnerWatermarking
---
