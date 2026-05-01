---
description: Noise reducer filter settings for spatial filter.
layout: schema
name: NoiseReducerSpatialFilterSettings
properties_list:
- description: ''
  name: PostFilterSharpenStrength
  type: object
- description: ''
  name: Speed
  type: object
- description: ''
  name: Strength
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-noise-reducer-spatial-filter-settings-schema.json
slug: mediaconvert-api-noise-reducer-spatial-filter-settings
source_filename: mediaconvert-api-noise-reducer-spatial-filter-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-noise-reducer-spatial-filter-settings-schema.json\",\n  \"title\": \"NoiseReducerSpatialFilterSettings\",\n  \"description\": \"Noise reducer filter settings for spatial filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PostFilterSharpenStrength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"postFilterSharpenStrength\"\n          },\n          \"description\": \"Specify strength of post noise reduction sharpening filter, with 0 disabling the filter and 3 enabling it at maximum strength.\"\n        }\n      ]\n    },\n    \"Speed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2Max3\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"speed\"\n          },\n          \"description\": \"The speed of the filter, from -2 (lower speed) to 3 (higher speed), with 0 being the nominal value.\"\n        }\n      ]\n    },\n    \"Strength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max16\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"strength\"\n          },\n          \"description\": \"Relative strength of noise reducing filter. Higher values produce stronger filtering.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-noise-reducer-spatial-filter-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: NoiseReducerSpatialFilterSettings
---
