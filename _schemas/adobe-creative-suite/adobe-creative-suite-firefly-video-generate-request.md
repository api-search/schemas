---
description: Request body for text-to-video generation
layout: schema
name: VideoGenerateRequest
properties_list:
- description: Text description of the video to generate
  name: prompt
  type: string
- description: Text describing what to avoid in the generated video
  name: negativePrompt
  type: string
- description: Output video dimensions
  name: size
  type: object
- description: Requested video duration in seconds
  name: duration
  type: number
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-video-generate-request-schema.json
slug: adobe-creative-suite-firefly-video-generate-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-video-generate-request-schema.json\",\n  \"title\": \"VideoGenerateRequest\",\n  \"description\": \"Request body for text-to-video generation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text description of the video to generate\",\n      \"maxLength\": 1024,\n      \"example\": \"A slow camera pan over a misty forest at dawn\"\n    },\n    \"negativePrompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text describing what to avoid in the generated video\",\n      \"maxLength\": 1024,\n      \"example\": \"example_value\"\n    },\n    \"size\": {\n      \"type\": \"object\",\n      \"description\": \"Output video dimensions\",\n      \"properties\": {\n        \"width\": {\n   \
  \       \"type\": \"integer\",\n          \"example\": 1920\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"example\": 1080\n        }\n      }\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"description\": \"Requested video duration in seconds\",\n      \"example\": 5.0\n    }\n  },\n  \"required\": [\n    \"prompt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-video-generate-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: VideoGenerateRequest
---
