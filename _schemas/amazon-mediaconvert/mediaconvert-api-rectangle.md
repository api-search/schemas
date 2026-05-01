---
description: Use Rectangle to identify a specific area of the video frame.
layout: schema
name: Rectangle
properties_list:
- description: ''
  name: Height
  type: object
- description: ''
  name: Width
  type: object
- description: ''
  name: X
  type: object
- description: ''
  name: Y
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-rectangle-schema.json
slug: mediaconvert-api-rectangle
source_filename: mediaconvert-api-rectangle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-rectangle-schema.json\",\n  \"title\": \"Rectangle\",\n  \"description\": \"Use Rectangle to identify a specific area of the video frame.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Height\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin2Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"height\"\n          },\n          \"description\": \"Height of rectangle in pixels. Specify only even numbers.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin2Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"width\"\n          },\n          \"description\": \"Width of rectangle in pixels.\
  \ Specify only even numbers.\"\n        }\n      ]\n    },\n    \"X\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"x\"\n          },\n          \"description\": \"The distance, in pixels, between the rectangle and the left edge of the video frame. Specify only even numbers.\"\n        }\n      ]\n    },\n    \"Y\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"y\"\n          },\n          \"description\": \"The distance, in pixels, between the rectangle and the top edge of the video frame. Specify only even numbers.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-rectangle-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Rectangle
---
