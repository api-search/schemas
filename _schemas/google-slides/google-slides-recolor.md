---
description: A recolor effect applied on an image.
layout: schema
name: Recolor
properties_list:
- description: The recolor effect is represented by a gradient.
  name: recolorStops
  type: array
- description: The name of the recolor effect.
  name: name
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-recolor-schema.json
slug: google-slides-recolor
source_filename: google-slides-recolor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Recolor\",\n  \"type\": \"object\",\n  \"description\": \"A recolor effect applied on an image.\\n\",\n  \"properties\": {\n    \"recolorStops\": {\n      \"type\": \"array\",\n      \"description\": \"The recolor effect is represented by a gradient.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the recolor effect.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-recolor-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Recolor
---
