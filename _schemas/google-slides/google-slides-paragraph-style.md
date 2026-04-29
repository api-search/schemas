---
description: Styles that apply to a whole paragraph. If this text is contained in a shape with a parent placeholder, then these paragraph styles may be inherited from the parent.
layout: schema
name: ParagraphStyle
properties_list:
- description: The amount of space between lines, as a percentage of normal, where normal is represented as 100.0.
  name: lineSpacing
  type: number
- description: The text alignment for this paragraph.
  name: alignment
  type: string
- description: The text direction of this paragraph.
  name: direction
  type: string
- description: The spacing mode for the paragraph.
  name: spacingMode
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-paragraph-style-schema.json
slug: google-slides-paragraph-style
source_filename: google-slides-paragraph-style-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ParagraphStyle\",\n  \"type\": \"object\",\n  \"description\": \"Styles that apply to a whole paragraph. If this text is contained in a shape with a parent placeholder, then these paragraph styles may be inherited from the parent.\\n\",\n  \"properties\": {\n    \"lineSpacing\": {\n      \"type\": \"number\",\n      \"description\": \"The amount of space between lines, as a percentage of normal, where normal is represented as 100.0.\\n\"\n    },\n    \"alignment\": {\n      \"type\": \"string\",\n      \"description\": \"The text alignment for this paragraph.\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"description\": \"The text direction of this paragraph.\"\n    },\n    \"spacingMode\": {\n      \"type\": \"string\",\n      \"description\": \"The spacing mode for the paragraph.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-paragraph-style-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: ParagraphStyle
---
