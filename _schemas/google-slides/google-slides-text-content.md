---
description: The general text content. The text must reside in a compatible shape (e.g., text box or rectangle) or a table cell in a page.
layout: schema
name: TextContent
properties_list:
- description: The text contents broken down into text elements.
  name: textElements
  type: array
- description: The bulleted lists contained in this text, keyed by list ID.
  name: lists
  type: object
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-text-content-schema.json
slug: google-slides-text-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextContent\",\n  \"type\": \"object\",\n  \"description\": \"The general text content. The text must reside in a compatible shape (e.g., text box or rectangle) or a table cell in a page.\\n\",\n  \"properties\": {\n    \"textElements\": {\n      \"type\": \"array\",\n      \"description\": \"The text contents broken down into text elements.\"\n    },\n    \"lists\": {\n      \"type\": \"object\",\n      \"description\": \"The bulleted lists contained in this text, keyed by list ID.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-text-content-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: TextContent
---
