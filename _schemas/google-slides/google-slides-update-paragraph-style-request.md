---
description: Updates the styling of paragraphs within a Shape or Table.
layout: schema
name: UpdateParagraphStyleRequest
properties_list:
- description: The object ID of the shape or table.
  name: objectId
  type: string
- description: The fields that should be updated.
  name: fields
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-update-paragraph-style-request-schema.json
slug: google-slides-update-paragraph-style-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateParagraphStyleRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the styling of paragraphs within a Shape or Table.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the shape or table.\"\n    },\n    \"fields\": {\n      \"type\": \"string\",\n      \"description\": \"The fields that should be updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-update-paragraph-style-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UpdateParagraphStyleRequest
---
