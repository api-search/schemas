---
description: Details regarding output
layout: schema
name: OutputDetail
properties_list:
- description: ''
  name: DurationInMs
  type: object
- description: ''
  name: VideoDetails
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-output-detail-schema.json
slug: mediaconvert-api-output-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-detail-schema.json\",\n  \"title\": \"OutputDetail\",\n  \"description\": \"Details regarding output\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DurationInMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"durationInMs\"\n          },\n          \"description\": \"Duration in milliseconds\"\n        }\n      ]\n    },\n    \"VideoDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoDetail\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoDetails\"\n          },\n          \"description\": \"Contains details about the output's video stream\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-detail-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OutputDetail
---
