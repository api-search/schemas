---
description: Create Dolby Vision Profile 5 or Profile 8.1 compatible video output.
layout: schema
name: DolbyVision
properties_list:
- description: ''
  name: L6Metadata
  type: object
- description: ''
  name: L6Mode
  type: object
- description: ''
  name: Mapping
  type: object
- description: ''
  name: Profile
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dolby-vision-schema.json
slug: mediaconvert-api-dolby-vision
source_filename: mediaconvert-api-dolby-vision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dolby-vision-schema.json\",\n  \"title\": \"DolbyVision\",\n  \"description\": \"Create Dolby Vision Profile 5 or Profile 8.1 compatible video output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"L6Metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DolbyVisionLevel6Metadata\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"l6Metadata\"\n          },\n          \"description\": \"Use these settings when you set DolbyVisionLevel6Mode to SPECIFY to override the MaxCLL and MaxFALL values in your input with new values.\"\n        }\n      ]\n    },\n    \"L6Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DolbyVisionLevel6Mode\"\n        },\n        {\n          \"xml\": {\n      \
  \      \"name\": \"l6Mode\"\n          },\n          \"description\": \"Use Dolby Vision Mode to choose how the service will handle Dolby Vision MaxCLL and MaxFALL properies.\"\n        }\n      ]\n    },\n    \"Mapping\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DolbyVisionMapping\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mapping\"\n          },\n          \"description\": \"Required when you set Dolby Vision Profile to Profile 8.1. When you set Content mapping to None, content mapping is not applied to the HDR10-compatible signal. Depending on the source peak nit level, clipping might occur on HDR devices without Dolby Vision. When you set Content mapping to HDR10 1000, the transcoder creates a 1,000 nits peak HDR10-compatible signal by applying static content mapping to the source. This mode is speed-optimized for PQ10 sources with metadata that is created from analysis. For graded Dolby Vision content, be aware that\
  \ creative intent might not be guaranteed with extreme 1,000 nits trims.\"\n        }\n      ]\n    },\n    \"Profile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DolbyVisionProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"profile\"\n          },\n          \"description\": \"Required when you enable Dolby Vision. Use Profile 5 to include frame-interleaved Dolby Vision metadata in your output. Your input must include Dolby Vision metadata or an HDR10 YUV color space. Use Profile 8.1 to include frame-interleaved Dolby Vision metadata and HDR10 metadata in your output. Your input must include Dolby Vision metadata.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dolby-vision-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DolbyVision
---
