---
description: Deletes text from a shape or a table cell.
layout: schema
name: DeleteTextRequest
properties_list:
- description: The object ID of the shape or table where the text will be deleted.
  name: objectId
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-delete-text-request-schema.json
slug: google-slides-delete-text-request
source_filename: google-slides-delete-text-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteTextRequest\",\n  \"type\": \"object\",\n  \"description\": \"Deletes text from a shape or a table cell.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the shape or table where the text will be deleted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-delete-text-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: DeleteTextRequest
---
