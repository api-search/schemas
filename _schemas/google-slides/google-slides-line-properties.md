---
description: The properties of a Line.
layout: schema
name: LineProperties
properties_list:
- description: The dash style of the line.
  name: dashStyle
  type: string
- description: The style of the arrow at the beginning of the line.
  name: startArrow
  type: string
- description: The style of the arrow at the end of the line.
  name: endArrow
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-line-properties-schema.json
slug: google-slides-line-properties
source_filename: google-slides-line-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LineProperties\",\n  \"type\": \"object\",\n  \"description\": \"The properties of a Line.\",\n  \"properties\": {\n    \"dashStyle\": {\n      \"type\": \"string\",\n      \"description\": \"The dash style of the line.\"\n    },\n    \"startArrow\": {\n      \"type\": \"string\",\n      \"description\": \"The style of the arrow at the beginning of the line.\"\n    },\n    \"endArrow\": {\n      \"type\": \"string\",\n      \"description\": \"The style of the arrow at the end of the line.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-line-properties-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: LineProperties
---
