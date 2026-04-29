---
description: Creates an image.
layout: schema
name: CreateImageRequest
properties_list:
- description: A user-supplied object ID.
  name: objectId
  type: string
- description: The image URL. The image is fetched once at insertion time and a copy is stored for display inside the presentation.
  name: url
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-create-image-request-schema.json
slug: google-slides-create-image-request
source_filename: google-slides-create-image-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateImageRequest\",\n  \"type\": \"object\",\n  \"description\": \"Creates an image.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"A user-supplied object ID.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The image URL. The image is fetched once at insertion time and a copy is stored for display inside the presentation.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-create-image-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: CreateImageRequest
---
