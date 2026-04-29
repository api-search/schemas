---
description: Represents a font family and weight of text.
layout: schema
name: WeightedFontFamily
properties_list:
- description: The font family of the text.
  name: fontFamily
  type: string
- description: The weight of the font. This field can have any value that is a multiple of 100 between 100 and 900, inclusive.
  name: weight
  type: integer
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-weighted-font-family-schema.json
slug: google-docs-v1-weighted-font-family
source_filename: google-docs-v1-weighted-font-family-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WeightedFontFamily\",\n  \"type\": \"object\",\n  \"description\": \"Represents a font family and weight of text.\",\n  \"properties\": {\n    \"fontFamily\": {\n      \"type\": \"string\",\n      \"description\": \"The font family of the text.\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"The weight of the font. This field can have any value that is a multiple of 100 between 100 and 900, inclusive.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-weighted-font-family-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: WeightedFontFamily
---
