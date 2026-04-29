---
description: Creates bullets for all of the paragraphs that overlap with a text range.
layout: schema
name: CreateParagraphBulletsRequest
properties_list:
- description: The object ID of the shape or table.
  name: objectId
  type: string
- description: The kinds of bullet glyphs to be used.
  name: bulletPreset
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-create-paragraph-bullets-request-schema.json
slug: google-slides-create-paragraph-bullets-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateParagraphBulletsRequest\",\n  \"type\": \"object\",\n  \"description\": \"Creates bullets for all of the paragraphs that overlap with a text range.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the shape or table.\"\n    },\n    \"bulletPreset\": {\n      \"type\": \"string\",\n      \"description\": \"The kinds of bullet glyphs to be used.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-create-paragraph-bullets-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: CreateParagraphBulletsRequest
---
