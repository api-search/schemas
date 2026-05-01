---
description: Contains details about the output's video stream
layout: schema
name: VideoDetail
properties_list:
- description: ''
  name: HeightInPx
  type: object
- description: ''
  name: WidthInPx
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-video-detail-schema.json
slug: mediaconvert-api-video-detail
source_filename: mediaconvert-api-video-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-video-detail-schema.json\",\n  \"title\": \"VideoDetail\",\n  \"description\": \"Contains details about the output's video stream\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HeightInPx\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"heightInPx\"\n          },\n          \"description\": \"Height in pixels for the output\"\n        }\n      ]\n    },\n    \"WidthInPx\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"widthInPx\"\n          },\n          \"description\": \"Width in pixels for the output\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-video-detail-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: VideoDetail
---
