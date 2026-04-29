---
description: An RGB color.
layout: schema
name: RgbColor
properties_list:
- description: The red component of the color, from 0.0 to 1.0.
  name: red
  type: number
- description: The green component of the color, from 0.0 to 1.0.
  name: green
  type: number
- description: The blue component of the color, from 0.0 to 1.0.
  name: blue
  type: number
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-rgb-color-schema.json
slug: google-slides-rgb-color
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RgbColor\",\n  \"type\": \"object\",\n  \"description\": \"An RGB color.\",\n  \"properties\": {\n    \"red\": {\n      \"type\": \"number\",\n      \"description\": \"The red component of the color, from 0.0 to 1.0.\"\n    },\n    \"green\": {\n      \"type\": \"number\",\n      \"description\": \"The green component of the color, from 0.0 to 1.0.\"\n    },\n    \"blue\": {\n      \"type\": \"number\",\n      \"description\": \"The blue component of the color, from 0.0 to 1.0.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-rgb-color-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: RgbColor
---
