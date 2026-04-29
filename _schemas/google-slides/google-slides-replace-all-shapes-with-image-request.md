---
description: Replaces all shapes that match the given criteria with the provided image.
layout: schema
name: ReplaceAllShapesWithImageRequest
properties_list:
- description: The image URL.
  name: imageUrl
  type: string
- description: The image replace method.
  name: imageReplaceMethod
  type: string
- description: If non-empty, limits to the given pages.
  name: pageObjectIds
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-replace-all-shapes-with-image-request-schema.json
slug: google-slides-replace-all-shapes-with-image-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplaceAllShapesWithImageRequest\",\n  \"type\": \"object\",\n  \"description\": \"Replaces all shapes that match the given criteria with the provided image.\\n\",\n  \"properties\": {\n    \"imageUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The image URL.\"\n    },\n    \"imageReplaceMethod\": {\n      \"type\": \"string\",\n      \"description\": \"The image replace method.\"\n    },\n    \"pageObjectIds\": {\n      \"type\": \"array\",\n      \"description\": \"If non-empty, limits to the given pages.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-replace-all-shapes-with-image-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: ReplaceAllShapesWithImageRequest
---
