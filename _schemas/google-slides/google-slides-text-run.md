---
description: A TextElement kind that represents a run of text that all has the same styling.
layout: schema
name: TextRun
properties_list:
- description: The text of this run.
  name: content
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-text-run-schema.json
slug: google-slides-text-run
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextRun\",\n  \"type\": \"object\",\n  \"description\": \"A TextElement kind that represents a run of text that all has the same styling.\\n\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The text of this run.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-text-run-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: TextRun
---
