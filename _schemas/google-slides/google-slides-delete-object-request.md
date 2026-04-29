---
description: Deletes an object, either pages or page elements, from the presentation.
layout: schema
name: DeleteObjectRequest
properties_list:
- description: The object ID of the page or page element to delete.
  name: objectId
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-delete-object-request-schema.json
slug: google-slides-delete-object-request
source_filename: google-slides-delete-object-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteObjectRequest\",\n  \"type\": \"object\",\n  \"description\": \"Deletes an object, either pages or page elements, from the presentation.\\n\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the page or page element to delete.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-delete-object-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: DeleteObjectRequest
---
