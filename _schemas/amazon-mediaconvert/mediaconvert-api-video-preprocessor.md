---
description: Find additional transcoding features under Preprocessors (VideoPreprocessors). Enable the features at each output individually. These features are disabled by default.
layout: schema
name: VideoPreprocessor
properties_list:
- description: ''
  name: ColorCorrector
  type: object
- description: ''
  name: Deinterlacer
  type: object
- description: ''
  name: DolbyVision
  type: object
- description: ''
  name: Hdr10Plus
  type: object
- description: ''
  name: ImageInserter
  type: object
- description: ''
  name: NoiseReducer
  type: object
- description: ''
  name: PartnerWatermarking
  type: object
- description: ''
  name: TimecodeBurnin
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-video-preprocessor-schema.json
slug: mediaconvert-api-video-preprocessor
source_filename: mediaconvert-api-video-preprocessor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-video-preprocessor-schema.json\",\n  \"title\": \"VideoPreprocessor\",\n  \"description\": \"Find additional transcoding features under Preprocessors (VideoPreprocessors). Enable the features at each output individually. These features are disabled by default.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ColorCorrector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColorCorrector\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorCorrector\"\n          },\n          \"description\": \"Use these settings to convert the color space or to modify properties such as hue and contrast for this output. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/converting-the-color-space.html.\"\n      \
  \  }\n      ]\n    },\n    \"Deinterlacer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Deinterlacer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deinterlacer\"\n          },\n          \"description\": \"Use the deinterlacer to produce smoother motion and a clearer picture. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/working-with-scan-type.html.\"\n        }\n      ]\n    },\n    \"DolbyVision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DolbyVision\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dolbyVision\"\n          },\n          \"description\": \"Enable Dolby Vision feature to produce Dolby Vision compatible video output.\"\n        }\n      ]\n    },\n    \"Hdr10Plus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Hdr10Plus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"\
  hdr10Plus\"\n          },\n          \"description\": \"Enable HDR10+ analyis and metadata injection. Compatible with HEVC only.\"\n        }\n      ]\n    },\n    \"ImageInserter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageInserter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageInserter\"\n          },\n          \"description\": \"Enable the Image inserter (ImageInserter) feature to include a graphic overlay on your video. Enable or disable this feature for each output individually. This setting is disabled by default.\"\n        }\n      ]\n    },\n    \"NoiseReducer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NoiseReducer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"noiseReducer\"\n          },\n          \"description\": \"Enable the Noise reducer feature to remove noise from your video output if necessary. Enable or disable this feature for each output\
  \ individually. This setting is disabled by default. When you enable Noise reducer, you must also select a value for Noise reducer filter. For AVC outputs, when you include Noise reducer, you cannot include the Bandwidth reduction filter.\"\n        }\n      ]\n    },\n    \"PartnerWatermarking\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartnerWatermarking\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"partnerWatermarking\"\n          },\n          \"description\": \"If you work with a third party video watermarking partner, use the group of settings that correspond with your watermarking partner to include watermarks in your output.\"\n        }\n      ]\n    },\n    \"TimecodeBurnin\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeBurnin\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeBurnin\"\n          },\n          \"description\": \"Settings for burning\
  \ the output timecode and specified prefix into the output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-video-preprocessor-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VideoPreprocessor
---
