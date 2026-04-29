---
description: A color and position in a gradient band.
layout: schema
name: ColorStop
properties_list:
- description: The alpha value of this color in the gradient band. Defaults to 1.0, fully opaque.
  name: alpha
  type: number
- description: The relative position of the color stop in the gradient band measured in percentage.
  name: position
  type: number
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-color-stop-schema.json
slug: google-slides-color-stop
source_filename: google-slides-color-stop-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ColorStop\",\n  \"type\": \"object\",\n  \"description\": \"A color and position in a gradient band.\",\n  \"properties\": {\n    \"alpha\": {\n      \"type\": \"number\",\n      \"description\": \"The alpha value of this color in the gradient band. Defaults to 1.0, fully opaque.\\n\"\n    },\n    \"position\": {\n      \"type\": \"number\",\n      \"description\": \"The relative position of the color stop in the gradient band measured in percentage.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-color-stop-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: ColorStop
---
