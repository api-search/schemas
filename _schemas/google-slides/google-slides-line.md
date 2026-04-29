---
description: A PageElement kind representing a non-connector line, straight connector, curved connector, or bent connector.
layout: schema
name: Line
properties_list:
- description: The category of the line.
  name: lineCategory
  type: string
- description: The type of the line.
  name: lineType
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-line-schema.json
slug: google-slides-line
source_filename: google-slides-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Line\",\n  \"type\": \"object\",\n  \"description\": \"A PageElement kind representing a non-connector line, straight connector, curved connector, or bent connector.\\n\",\n  \"properties\": {\n    \"lineCategory\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the line.\"\n    },\n    \"lineType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the line.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-line-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Line
---
