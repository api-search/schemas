---
description: Represents the styling that can be applied to a TextRun. If this text is contained in a shape with a parent placeholder, then these text styles may be inherited from the parent.
layout: schema
name: TextStyle
properties_list:
- description: Whether the text is bold.
  name: bold
  type: boolean
- description: Whether the text is italicized.
  name: italic
  type: boolean
- description: The font family of the text.
  name: fontFamily
  type: string
- description: The text's vertical offset from its normal position.
  name: baselineOffset
  type: string
- description: Whether the text is in small capital letters.
  name: smallCaps
  type: boolean
- description: Whether the text is struck through.
  name: strikethrough
  type: boolean
- description: Whether the text is underlined.
  name: underline
  type: boolean
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-text-style-schema.json
slug: google-slides-text-style
source_filename: google-slides-text-style-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextStyle\",\n  \"type\": \"object\",\n  \"description\": \"Represents the styling that can be applied to a TextRun. If this text is contained in a shape with a parent placeholder, then these text styles may be inherited from the parent.\\n\",\n  \"properties\": {\n    \"bold\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text is bold.\"\n    },\n    \"italic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text is italicized.\"\n    },\n    \"fontFamily\": {\n      \"type\": \"string\",\n      \"description\": \"The font family of the text.\"\n    },\n    \"baselineOffset\": {\n      \"type\": \"string\",\n      \"description\": \"The text's vertical offset from its normal position.\"\n    },\n    \"smallCaps\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text is in small capital letters.\"\n    },\n    \"strikethrough\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text is struck through.\"\n    },\n    \"underline\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text is underlined.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-text-style-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: TextStyle
---
