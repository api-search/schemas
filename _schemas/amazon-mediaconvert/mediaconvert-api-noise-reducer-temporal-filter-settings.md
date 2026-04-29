---
description: Noise reducer filter settings for temporal filter.
layout: schema
name: NoiseReducerTemporalFilterSettings
properties_list:
- description: ''
  name: AggressiveMode
  type: object
- description: ''
  name: PostTemporalSharpening
  type: object
- description: ''
  name: PostTemporalSharpeningStrength
  type: object
- description: ''
  name: Speed
  type: object
- description: ''
  name: Strength
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-noise-reducer-temporal-filter-settings-schema.json
slug: mediaconvert-api-noise-reducer-temporal-filter-settings
source_filename: mediaconvert-api-noise-reducer-temporal-filter-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-noise-reducer-temporal-filter-settings-schema.json\",\n  \"title\": \"NoiseReducerTemporalFilterSettings\",\n  \"description\": \"Noise reducer filter settings for temporal filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AggressiveMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max4\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"aggressiveMode\"\n          },\n          \"description\": \"Use Aggressive mode for content that has complex motion. Higher values produce stronger temporal filtering. This filters highly complex scenes more aggressively and creates better VQ for low bitrate outputs.\"\n        }\n      ]\n    },\n    \"PostTemporalSharpening\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/NoiseFilterPostTemporalSharpening\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"postTemporalSharpening\"\n          },\n          \"description\": \"When you set Noise reducer (noiseReducer) to Temporal (TEMPORAL), the bandwidth and sharpness of your output is reduced. You can optionally use Post temporal sharpening (postTemporalSharpening) to apply sharpening to the edges of your output. Note that Post temporal sharpening will also make the bandwidth reduction from the Noise reducer smaller. The default behavior, Auto (AUTO), allows the transcoder to determine whether to apply sharpening, depending on your input type and quality. When you set Post temporal sharpening to Enabled (ENABLED), specify how much sharpening is applied using Post temporal sharpening strength (postTemporalSharpeningStrength). Set Post temporal sharpening to Disabled (DISABLED) to not apply sharpening.\"\n        }\n      ]\n    },\n    \"PostTemporalSharpeningStrength\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NoiseFilterPostTemporalSharpeningStrength\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"postTemporalSharpeningStrength\"\n          },\n          \"description\": \"Use Post temporal sharpening strength (postTemporalSharpeningStrength) to define the amount of sharpening the transcoder applies to your output. Set Post temporal sharpening strength to Low (LOW), Medium (MEDIUM), or High (HIGH) to indicate the amount of sharpening.\"\n        }\n      ]\n    },\n    \"Speed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative1Max3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"speed\"\n          },\n          \"description\": \"The speed of the filter (higher number is faster). Low setting reduces bit rate at the cost of transcode time, high setting improves transcode time at the cost of bit rate.\"\n        }\n  \
  \    ]\n    },\n    \"Strength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max16\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"strength\"\n          },\n          \"description\": \"Specify the strength of the noise reducing filter on this output. Higher values produce stronger filtering. We recommend the following value ranges, depending on the result that you want: * 0-2 for complexity reduction with minimal sharpness loss * 2-8 for complexity reduction with image preservation * 8-16 for a high level of complexity reduction\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-noise-reducer-temporal-filter-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NoiseReducerTemporalFilterSettings
---
