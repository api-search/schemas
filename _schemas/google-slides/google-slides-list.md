---
description: A list describes the look and feel of bullets belonging to paragraphs.
layout: schema
name: List
properties_list:
- description: The ID of the list.
  name: listId
  type: string
- description: A map of nesting levels to the properties of bullets at the associated level.
  name: nestingLevel
  type: object
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-list-schema.json
slug: google-slides-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"List\",\n  \"type\": \"object\",\n  \"description\": \"A list describes the look and feel of bullets belonging to paragraphs.\",\n  \"properties\": {\n    \"listId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the list.\"\n    },\n    \"nestingLevel\": {\n      \"type\": \"object\",\n      \"description\": \"A map of nesting levels to the properties of bullets at the associated level.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-list-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: List
---
