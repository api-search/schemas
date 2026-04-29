---
description: Specify the offset between the upper-left corner of the video frame and the top left corner of the overlay.
layout: schema
name: MotionImageInsertionOffset
properties_list:
- description: ''
  name: ImageX
  type: object
- description: ''
  name: ImageY
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-motion-image-insertion-offset-schema.json
slug: mediaconvert-api-motion-image-insertion-offset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-motion-image-insertion-offset-schema.json\",\n  \"title\": \"MotionImageInsertionOffset\",\n  \"description\": \"Specify the offset between the upper-left corner of the video frame and the top left corner of the overlay.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImageX\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageX\"\n          },\n          \"description\": \"Set the distance, in pixels, between the overlay and the left edge of the video frame.\"\n        }\n      ]\n    },\n    \"ImageY\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"\
  xml\": {\n            \"name\": \"imageY\"\n          },\n          \"description\": \"Set the distance, in pixels, between the overlay and the top edge of the video frame.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-motion-image-insertion-offset-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MotionImageInsertionOffset
---
