---
description: The properties of an Image.
layout: schema
name: ImageProperties
properties_list:
- description: The transparency effect of the image. The value should be in the interval [0.0, 1.0], where 0 means no effect and 1 means completely transparent.
  name: transparency
  type: number
- description: The brightness effect of the image. The value should be in the interval [-1.0, 1.0], where 0 means no effect.
  name: brightness
  type: number
- description: The contrast effect of the image. The value should be in the interval [-1.0, 1.0], where 0 means no effect.
  name: contrast
  type: number
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-image-properties-schema.json
slug: google-slides-image-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImageProperties\",\n  \"type\": \"object\",\n  \"description\": \"The properties of an Image.\",\n  \"properties\": {\n    \"transparency\": {\n      \"type\": \"number\",\n      \"description\": \"The transparency effect of the image. The value should be in the interval [0.0, 1.0], where 0 means no effect and 1 means completely transparent.\\n\"\n    },\n    \"brightness\": {\n      \"type\": \"number\",\n      \"description\": \"The brightness effect of the image. The value should be in the interval [-1.0, 1.0], where 0 means no effect.\\n\"\n    },\n    \"contrast\": {\n      \"type\": \"number\",\n      \"description\": \"The contrast effect of the image. The value should be in the interval [-1.0, 1.0], where 0 means no effect.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-image-properties-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: ImageProperties
---
