---
description: Represents the styling that can be applied to text. Inherited text styles are represented as unset fields. A text style's parent depends on where the text style is defined.
layout: schema
name: TextStyle
properties_list:
- description: Whether the text is bold.
  name: bold
  type: boolean
- description: Whether the text is italicized.
  name: italic
  type: boolean
- description: Whether the text is underlined.
  name: underline
  type: boolean
- description: Whether the text is struck through.
  name: strikethrough
  type: boolean
- description: Whether the text is in small capital letters.
  name: smallCaps
  type: boolean
- description: The text's vertical offset from its normal position.
  name: baselineOffset
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-text-style-schema.json
slug: google-docs-v1-text-style
source_filename: google-docs-v1-text-style-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextStyle\",\n  \"type\": \"object\",\n  \"description\": \"Represents the styling that can be applied to text. Inherited text styles are represented as unset fields. A text style's parent depends on where the text style is defined.\",\n  \"properties\": {\n    \"bold\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text is bold.\"\n    },\n    \"italic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text is italicized.\"\n    },\n    \"underline\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text is underlined.\"\n    },\n    \"strikethrough\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text is struck through.\"\n    },\n    \"smallCaps\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text is in small capital letters.\"\n    },\n    \"baselineOffset\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The text's vertical offset from its normal position.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-text-style-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TextStyle
---
