---
description: The palette of predefined colors for a page.
layout: schema
name: ColorScheme
properties_list:
- description: The ThemeColorType and corresponding concrete color pairs.
  name: colors
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-color-scheme-schema.json
slug: google-slides-color-scheme
source_filename: google-slides-color-scheme-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ColorScheme\",\n  \"type\": \"object\",\n  \"description\": \"The palette of predefined colors for a page.\\n\",\n  \"properties\": {\n    \"colors\": {\n      \"type\": \"array\",\n      \"description\": \"The ThemeColorType and corresponding concrete color pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-color-scheme-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: ColorScheme
---
