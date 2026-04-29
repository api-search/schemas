---
description: Styles that apply to a whole paragraph. Inherited paragraph styles are represented as unset fields.
layout: schema
name: ParagraphStyle
properties_list:
- description: The heading ID of the paragraph.
  name: headingId
  type: string
- description: The named style type of the paragraph.
  name: namedStyleType
  type: string
- description: The text alignment for this paragraph.
  name: alignment
  type: string
- description: The amount of space between lines as a percentage of normal, where normal is represented as 100.0.
  name: lineSpacing
  type: number
- description: The text direction of this paragraph.
  name: direction
  type: string
- description: The spacing mode for the paragraph.
  name: spacingMode
  type: string
- description: A list of the tab stops for this paragraph, sorted in ascending order of the tab stop offset.
  name: tabStops
  type: array
- description: Whether all lines of the paragraph should be laid out on the same page or column if possible.
  name: keepLinesTogether
  type: boolean
- description: Whether at least a part of this paragraph should be laid out on the same page or column as the next paragraph if possible.
  name: keepWithNext
  type: boolean
- description: Whether to avoid widows and orphans for the paragraph.
  name: avoidWidowAndOrphan
  type: boolean
- description: Whether the current paragraph should always start at the beginning of a page.
  name: pageBreakBefore
  type: boolean
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-paragraph-style-schema.json
slug: google-docs-v1-paragraph-style
source_filename: google-docs-v1-paragraph-style-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ParagraphStyle\",\n  \"type\": \"object\",\n  \"description\": \"Styles that apply to a whole paragraph. Inherited paragraph styles are represented as unset fields.\",\n  \"properties\": {\n    \"headingId\": {\n      \"type\": \"string\",\n      \"description\": \"The heading ID of the paragraph.\"\n    },\n    \"namedStyleType\": {\n      \"type\": \"string\",\n      \"description\": \"The named style type of the paragraph.\"\n    },\n    \"alignment\": {\n      \"type\": \"string\",\n      \"description\": \"The text alignment for this paragraph.\"\n    },\n    \"lineSpacing\": {\n      \"type\": \"number\",\n      \"description\": \"The amount of space between lines as a percentage of normal, where normal is represented as 100.0.\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"description\": \"The text direction of this paragraph.\"\n    },\n    \"spacingMode\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The spacing mode for the paragraph.\"\n    },\n    \"tabStops\": {\n      \"type\": \"array\",\n      \"description\": \"A list of the tab stops for this paragraph, sorted in ascending order of the tab stop offset.\"\n    },\n    \"keepLinesTogether\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether all lines of the paragraph should be laid out on the same page or column if possible.\"\n    },\n    \"keepWithNext\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether at least a part of this paragraph should be laid out on the same page or column as the next paragraph if possible.\"\n    },\n    \"avoidWidowAndOrphan\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to avoid widows and orphans for the paragraph.\"\n    },\n    \"pageBreakBefore\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the current paragraph should always start at the beginning of a page.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-paragraph-style-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: ParagraphStyle
---
