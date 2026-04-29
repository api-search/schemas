---
description: Creates a video.
layout: schema
name: CreateVideoRequest
properties_list:
- description: A user-supplied object ID.
  name: objectId
  type: string
- description: The video source.
  name: source
  type: string
- description: The video source's unique identifier for this video.
  name: id
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-create-video-request-schema.json
slug: google-slides-create-video-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateVideoRequest\",\n  \"type\": \"object\",\n  \"description\": \"Creates a video.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"A user-supplied object ID.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The video source.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The video source's unique identifier for this video.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-create-video-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: CreateVideoRequest
---
