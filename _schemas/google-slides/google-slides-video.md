---
description: A PageElement kind representing a video.
layout: schema
name: Video
properties_list:
- description: An URL to a video. The URL is valid as long as the source video exists and sharing settings do not change.
  name: url
  type: string
- description: The video source.
  name: source
  type: string
- description: The video source's unique identifier for this video.
  name: id
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-video-schema.json
slug: google-slides-video
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Video\",\n  \"type\": \"object\",\n  \"description\": \"A PageElement kind representing a video.\\n\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"An URL to a video. The URL is valid as long as the source video exists and sharing settings do not change.\\n\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The video source.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The video source's unique identifier for this video.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-video-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Video
---
