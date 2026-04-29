---
description: A TextElement describes the content of a range of indices in the text content of a Shape or TableCell.
layout: schema
name: TextElement
properties_list:
- description: The zero-based start index of this text element, in Unicode code units of the UTF-16 encoding.
  name: startIndex
  type: integer
- description: The zero-based end index of this text element, exclusive, in Unicode code units of the UTF-16 encoding.
  name: endIndex
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-text-element-schema.json
slug: google-slides-text-element
source_filename: google-slides-text-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextElement\",\n  \"type\": \"object\",\n  \"description\": \"A TextElement describes the content of a range of indices in the text content of a Shape or TableCell.\\n\",\n  \"properties\": {\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based start index of this text element, in Unicode code units of the UTF-16 encoding.\\n\"\n    },\n    \"endIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based end index of this text element, exclusive, in Unicode code units of the UTF-16 encoding.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-text-element-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: TextElement
---
