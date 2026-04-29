---
description: A solid color fill.
layout: schema
name: SolidFill
properties_list:
- description: The fraction of this color that should be applied to the pixel. The final pixel color is defined by the equation pixel_color = alpha * this_color + (1.0 - alpha) * pixel_color. Value is in [0.0, 1.0].
  name: alpha
  type: number
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-solid-fill-schema.json
slug: google-slides-solid-fill
source_filename: google-slides-solid-fill-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SolidFill\",\n  \"type\": \"object\",\n  \"description\": \"A solid color fill.\",\n  \"properties\": {\n    \"alpha\": {\n      \"type\": \"number\",\n      \"description\": \"The fraction of this color that should be applied to the pixel. The final pixel color is defined by the equation pixel_color = alpha * this_color + (1.0 - alpha) * pixel_color. Value is in [0.0, 1.0].\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-solid-fill-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: SolidFill
---
