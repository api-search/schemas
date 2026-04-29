---
description: Replaces an existing image with a new image.
layout: schema
name: ReplaceImageRequest
properties_list:
- description: The ID of the existing image that will be replaced.
  name: imageObjectId
  type: string
- description: The URL of the new image.
  name: url
  type: string
- description: The replace method.
  name: imageReplaceMethod
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-replace-image-request-schema.json
slug: google-slides-replace-image-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplaceImageRequest\",\n  \"type\": \"object\",\n  \"description\": \"Replaces an existing image with a new image.\",\n  \"properties\": {\n    \"imageObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the existing image that will be replaced.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the new image.\"\n    },\n    \"imageReplaceMethod\": {\n      \"type\": \"string\",\n      \"description\": \"The replace method.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-replace-image-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: ReplaceImageRequest
---
