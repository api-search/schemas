---
description: Specifies a contiguous range of an indexed collection.
layout: schema
name: Range
properties_list:
- description: The optional zero-based start index of the collection.
  name: startIndex
  type: integer
- description: The optional zero-based end index of the collection.
  name: endIndex
  type: integer
- description: The type of range.
  name: type
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-range-schema.json
slug: google-slides-range
source_filename: google-slides-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Range\",\n  \"type\": \"object\",\n  \"description\": \"Specifies a contiguous range of an indexed collection.\",\n  \"properties\": {\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The optional zero-based start index of the collection.\"\n    },\n    \"endIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The optional zero-based end index of the collection.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of range.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-range-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Range
---
