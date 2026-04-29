---
description: Update the styling of text in a Shape or Table.
layout: schema
name: UpdateTextStyleRequest
properties_list:
- description: The object ID of the shape or table with the text to be styled.
  name: objectId
  type: string
- description: The fields that should be updated.
  name: fields
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-update-text-style-request-schema.json
slug: google-slides-update-text-style-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateTextStyleRequest\",\n  \"type\": \"object\",\n  \"description\": \"Update the styling of text in a Shape or Table.\\n\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the shape or table with the text to be styled.\"\n    },\n    \"fields\": {\n      \"type\": \"string\",\n      \"description\": \"The fields that should be updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-update-text-style-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UpdateTextStyleRequest
---
