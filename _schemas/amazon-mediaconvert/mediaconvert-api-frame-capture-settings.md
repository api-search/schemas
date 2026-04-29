---
description: Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value FRAME_CAPTURE.
layout: schema
name: FrameCaptureSettings
properties_list:
- description: ''
  name: FramerateDenominator
  type: object
- description: ''
  name: FramerateNumerator
  type: object
- description: ''
  name: MaxCaptures
  type: object
- description: ''
  name: Quality
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-frame-capture-settings-schema.json
slug: mediaconvert-api-frame-capture-settings
source_filename: mediaconvert-api-frame-capture-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-frame-capture-settings-schema.json\",\n  \"title\": \"FrameCaptureSettings\",\n  \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value FRAME_CAPTURE.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FramerateDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateDenominator\"\n          },\n          \"description\": \"Frame capture will encode the first frame of the output stream, then one frame every framerateDenominator/framerateNumerator seconds. For example, settings of framerateNumerator = 1 and framerateDenominator = 3 (a rate of 1/3 frame per second) will capture the first frame,\
  \ then 1 frame every 3s. Files will be named as filename.n.jpg where n is the 0-based sequence number of each Capture.\"\n        }\n      ]\n    },\n    \"FramerateNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateNumerator\"\n          },\n          \"description\": \"Frame capture will encode the first frame of the output stream, then one frame every framerateDenominator/framerateNumerator seconds. For example, settings of framerateNumerator = 1 and framerateDenominator = 3 (a rate of 1/3 frame per second) will capture the first frame, then 1 frame every 3s. Files will be named as filename.NNNNNNN.jpg where N is the 0-based frame sequence number zero padded to 7 decimal places.\"\n        }\n      ]\n    },\n    \"MaxCaptures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max10000000\"\n    \
  \    },\n        {\n          \"xml\": {\n            \"name\": \"maxCaptures\"\n          },\n          \"description\": \"Maximum number of captures (encoded jpg output files).\"\n        }\n      ]\n    },\n    \"Quality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"quality\"\n          },\n          \"description\": \"JPEG Quality - a higher value equals higher quality.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-frame-capture-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: FrameCaptureSettings
---
