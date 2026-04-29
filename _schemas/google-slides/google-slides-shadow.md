---
description: The shadow properties of a page element.
layout: schema
name: Shadow
properties_list:
- description: The type of the shadow.
  name: type
  type: string
- description: The alignment point of the shadow.
  name: alignment
  type: string
- description: The alpha of the shadow's color, from 0.0 to 1.0.
  name: alpha
  type: number
- description: Whether the shadow should rotate with the shape.
  name: rotateWithShape
  type: boolean
- description: The shadow property state.
  name: propertyState
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-shadow-schema.json
slug: google-slides-shadow
source_filename: google-slides-shadow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Shadow\",\n  \"type\": \"object\",\n  \"description\": \"The shadow properties of a page element.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the shadow.\"\n    },\n    \"alignment\": {\n      \"type\": \"string\",\n      \"description\": \"The alignment point of the shadow.\"\n    },\n    \"alpha\": {\n      \"type\": \"number\",\n      \"description\": \"The alpha of the shadow's color, from 0.0 to 1.0.\\n\"\n    },\n    \"rotateWithShape\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the shadow should rotate with the shape.\"\n    },\n    \"propertyState\": {\n      \"type\": \"string\",\n      \"description\": \"The shadow property state.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-shadow-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Shadow
---
