---
description: A magnitude in a single direction in the specified units.
layout: schema
name: Dimension
properties_list:
- description: The magnitude.
  name: magnitude
  type: number
- description: The units for the magnitude.
  name: unit
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-dimension-schema.json
slug: google-slides-dimension
source_filename: google-slides-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Dimension\",\n  \"type\": \"object\",\n  \"description\": \"A magnitude in a single direction in the specified units.\",\n  \"properties\": {\n    \"magnitude\": {\n      \"type\": \"number\",\n      \"description\": \"The magnitude.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The units for the magnitude.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-dimension-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Dimension
---
