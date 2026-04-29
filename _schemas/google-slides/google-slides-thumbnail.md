---
description: The thumbnail of a page.
layout: schema
name: Thumbnail
properties_list:
- description: The content URL of the thumbnail image. The URL to the image has a default lifetime of 30 minutes. This URL is tagged with the account of the requester.
  name: contentUrl
  type: string
- description: The positive width in pixels of the thumbnail image.
  name: width
  type: integer
- description: The positive height in pixels of the thumbnail image.
  name: height
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-thumbnail-schema.json
slug: google-slides-thumbnail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Thumbnail\",\n  \"type\": \"object\",\n  \"description\": \"The thumbnail of a page.\",\n  \"properties\": {\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The content URL of the thumbnail image. The URL to the image has a default lifetime of 30 minutes. This URL is tagged with the account of the requester.\\n\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"The positive width in pixels of the thumbnail image.\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"The positive height in pixels of the thumbnail image.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-thumbnail-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Thumbnail
---
