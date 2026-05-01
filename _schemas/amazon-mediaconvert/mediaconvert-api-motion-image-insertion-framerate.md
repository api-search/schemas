---
description: For motion overlays that don't have a built-in frame rate, specify the frame rate of the overlay in frames per second, as a fraction. For example, specify 24 fps as 24/1. The overlay frame rate doesn't need to match the frame rate of the underlying video.
layout: schema
name: MotionImageInsertionFramerate
properties_list:
- description: ''
  name: FramerateDenominator
  type: object
- description: ''
  name: FramerateNumerator
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-motion-image-insertion-framerate-schema.json
slug: mediaconvert-api-motion-image-insertion-framerate
source_filename: mediaconvert-api-motion-image-insertion-framerate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-motion-image-insertion-framerate-schema.json\",\n  \"title\": \"MotionImageInsertionFramerate\",\n  \"description\": \"For motion overlays that don't have a built-in frame rate, specify the frame rate of the overlay in frames per second, as a fraction. For example, specify 24 fps as 24/1. The overlay frame rate doesn't need to match the frame rate of the underlying video.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FramerateDenominator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max17895697\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateDenominator\"\n          },\n          \"description\": \"The bottom of the fraction that expresses your overlay frame rate. For example, if your frame rate\
  \ is 24 fps, set this value to 1.\"\n        }\n      ]\n    },\n    \"FramerateNumerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483640\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerateNumerator\"\n          },\n          \"description\": \"The top of the fraction that expresses your overlay frame rate. For example, if your frame rate is 24 fps, set this value to 24.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-motion-image-insertion-framerate-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MotionImageInsertionFramerate
---
