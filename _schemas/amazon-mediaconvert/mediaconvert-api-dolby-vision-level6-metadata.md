---
description: Use these settings when you set DolbyVisionLevel6Mode to SPECIFY to override the MaxCLL and MaxFALL values in your input with new values.
layout: schema
name: DolbyVisionLevel6Metadata
properties_list:
- description: ''
  name: MaxCll
  type: object
- description: ''
  name: MaxFall
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dolby-vision-level6-metadata-schema.json
slug: mediaconvert-api-dolby-vision-level6-metadata
source_filename: mediaconvert-api-dolby-vision-level6-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dolby-vision-level6-metadata-schema.json\",\n  \"title\": \"DolbyVisionLevel6Metadata\",\n  \"description\": \"Use these settings when you set DolbyVisionLevel6Mode to SPECIFY to override the MaxCLL and MaxFALL values in your input with new values.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxCll\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxCll\"\n          },\n          \"description\": \"Maximum Content Light Level. Static HDR metadata that corresponds to the brightest pixel in the entire stream. Measured in nits.\"\n        }\n      ]\n    },\n    \"MaxFall\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"maxFall\"\n          },\n          \"description\": \"Maximum Frame-Average Light Level. Static HDR metadata that corresponds to the highest frame-average brightness in the entire stream. Measured in nits.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dolby-vision-level6-metadata-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DolbyVisionLevel6Metadata
---
