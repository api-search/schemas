---
description: The autofit properties of a Shape.
layout: schema
name: Autofit
properties_list:
- description: The autofit type of the shape.
  name: autofitType
  type: string
- description: The font scale applied to the shape. For shapes with autofit enabled, this is the font scale value applied by the auto-fit algorithm.
  name: fontScale
  type: number
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-autofit-schema.json
slug: google-slides-autofit
source_filename: google-slides-autofit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Autofit\",\n  \"type\": \"object\",\n  \"description\": \"The autofit properties of a Shape.\",\n  \"properties\": {\n    \"autofitType\": {\n      \"type\": \"string\",\n      \"description\": \"The autofit type of the shape.\"\n    },\n    \"fontScale\": {\n      \"type\": \"number\",\n      \"description\": \"The font scale applied to the shape. For shapes with autofit enabled, this is the font scale value applied by the auto-fit algorithm.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-autofit-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Autofit
---
