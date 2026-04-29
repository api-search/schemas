---
description: Caption Rectangle
layout: schema
name: CaptionRectangle
properties_list:
- description: ''
  name: Height
  type: object
- description: ''
  name: LeftOffset
  type: object
- description: ''
  name: TopOffset
  type: object
- description: ''
  name: Width
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-caption-rectangle-schema.json
slug: medialive-api-caption-rectangle
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-rectangle-schema.json\",\n  \"title\": \"CaptionRectangle\",\n  \"description\": \"Caption Rectangle\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Height\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"height\"\n          },\n          \"description\": \"See the description in leftOffset.\\nFor height, specify the entire height of the rectangle as a percentage of the underlying frame height. For example, \\\\\\\"80\\\\\\\" means the rectangle height is 80% of the underlying frame height. The topOffset and rectangleHeight must add up to 100% or less.\\nThis field corresponds to tts:extent - Y in the TTML standard.\"\n        }\n      ]\n    },\n    \"\
  LeftOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"leftOffset\"\n          },\n          \"description\": \"Applies only if you plan to convert these source captions to EBU-TT-D or TTML in an output. (Make sure to leave the default if you don't have either of these formats in the output.) You can define a display rectangle for the captions that is smaller than the underlying video frame. You define the rectangle by specifying the position of the left edge, top edge, bottom edge, and right edge of the rectangle, all within the underlying video frame. The units for the measurements are percentages.\\nIf you specify a value for one of these fields, you must specify a value for all of them.\\nFor leftOffset, specify the position of the left edge of the rectangle, as a percentage of the underlying frame width, and relative to the left edge of the frame. For example,\
  \ \\\\\\\"10\\\\\\\" means the measurement is 10% of the underlying frame width. The rectangle left edge starts at that position from the left edge of the frame.\\nThis field corresponds to tts:origin - X in the TTML standard.\"\n        }\n      ]\n    },\n    \"TopOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"topOffset\"\n          },\n          \"description\": \"See the description in leftOffset.\\nFor topOffset, specify the position of the top edge of the rectangle, as a percentage of the underlying frame height, and relative to the top edge of the frame. For example, \\\\\\\"10\\\\\\\" means the measurement is 10% of the underlying frame height. The rectangle top edge starts at that position from the top edge of the frame.\\nThis field corresponds to tts:origin - Y in the TTML standard.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"width\"\n          },\n          \"description\": \"See the description in leftOffset.\\nFor width, specify the entire width of the rectangle as a percentage of the underlying frame width. For example, \\\\\\\"80\\\\\\\" means the rectangle width is 80% of the underlying frame width. The leftOffset and rectangleWidth must add up to 100% or less.\\nThis field corresponds to tts:extent - X in the TTML standard.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TopOffset\",\n    \"Height\",\n    \"Width\",\n    \"LeftOffset\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-rectangle-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CaptionRectangle
---
