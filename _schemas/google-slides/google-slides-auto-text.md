---
description: A TextElement kind that represents auto text.
layout: schema
name: AutoText
properties_list:
- description: The type of this auto text.
  name: type
  type: string
- description: The rendered content of this auto text, if available.
  name: content
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-auto-text-schema.json
slug: google-slides-auto-text
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutoText\",\n  \"type\": \"object\",\n  \"description\": \"A TextElement kind that represents auto text.\\n\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of this auto text.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The rendered content of this auto text, if available.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-auto-text-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: AutoText
---
