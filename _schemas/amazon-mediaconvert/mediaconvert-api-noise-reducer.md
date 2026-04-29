---
description: Enable the Noise reducer feature to remove noise from your video output if necessary. Enable or disable this feature for each output individually. This setting is disabled by default. When you enable Noise reducer, you must also select a value for Noise reducer filter. For AVC outputs, when you include Noise reducer, you cannot include the Bandwidth reduction filter.
layout: schema
name: NoiseReducer
properties_list:
- description: ''
  name: Filter
  type: object
- description: ''
  name: FilterSettings
  type: object
- description: ''
  name: SpatialFilterSettings
  type: object
- description: ''
  name: TemporalFilterSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-noise-reducer-schema.json
slug: mediaconvert-api-noise-reducer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-noise-reducer-schema.json\",\n  \"title\": \"NoiseReducer\",\n  \"description\": \"Enable the Noise reducer feature to remove noise from your video output if necessary. Enable or disable this feature for each output individually. This setting is disabled by default. When you enable Noise reducer, you must also select a value for Noise reducer filter. For AVC outputs, when you include Noise reducer, you cannot include the Bandwidth reduction filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NoiseReducerFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filter\"\n          },\n          \"description\": \"Use Noise reducer filter (NoiseReducerFilter) to select\
  \ one of the following spatial image filtering functions. To use this setting, you must also enable Noise reducer (NoiseReducer). * Bilateral preserves edges while reducing noise. * Mean (softest), Gaussian, Lanczos, and Sharpen (sharpest) do convolution filtering. * Conserve does min/max noise reduction. * Spatial does frequency-domain filtering based on JND principles. * Temporal optimizes video quality for complex motion.\"\n        }\n      ]\n    },\n    \"FilterSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NoiseReducerFilterSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterSettings\"\n          },\n          \"description\": \"Settings for a noise reducer filter\"\n        }\n      ]\n    },\n    \"SpatialFilterSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NoiseReducerSpatialFilterSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\":\
  \ \"spatialFilterSettings\"\n          },\n          \"description\": \"Noise reducer filter settings for spatial filter.\"\n        }\n      ]\n    },\n    \"TemporalFilterSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NoiseReducerTemporalFilterSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"temporalFilterSettings\"\n          },\n          \"description\": \"Noise reducer filter settings for temporal filter.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-noise-reducer-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NoiseReducer
---
