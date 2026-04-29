---
description: A hypertext link.
layout: schema
name: Link
properties_list:
- description: If set, indicates this is a link to the external web page at this URL.
  name: url
  type: string
- description: If set, indicates this is a link to a slide in this presentation, addressed by its position.
  name: relativeLink
  type: string
- description: If set, indicates this is a link to the specific page in this presentation with this ID.
  name: pageObjectId
  type: string
- description: If set, indicates this is a link to the slide at this zero-based index in the presentation.
  name: slideIndex
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-link-schema.json
slug: google-slides-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Link\",\n  \"type\": \"object\",\n  \"description\": \"A hypertext link.\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"If set, indicates this is a link to the external web page at this URL.\"\n    },\n    \"relativeLink\": {\n      \"type\": \"string\",\n      \"description\": \"If set, indicates this is a link to a slide in this presentation, addressed by its position.\\n\"\n    },\n    \"pageObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"If set, indicates this is a link to the specific page in this presentation with this ID.\\n\"\n    },\n    \"slideIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"If set, indicates this is a link to the slide at this zero-based index in the presentation.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-link-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Link
---
