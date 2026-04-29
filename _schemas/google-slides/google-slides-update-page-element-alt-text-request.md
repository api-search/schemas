---
description: Updates the alt text title and/or description of a page element.
layout: schema
name: UpdatePageElementAltTextRequest
properties_list:
- description: The object ID of the page element.
  name: objectId
  type: string
- description: The updated alt text title of the page element.
  name: title
  type: string
- description: The updated alt text description of the page element.
  name: description
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-update-page-element-alt-text-request-schema.json
slug: google-slides-update-page-element-alt-text-request
source_filename: google-slides-update-page-element-alt-text-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdatePageElementAltTextRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the alt text title and/or description of a page element.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the page element.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The updated alt text title of the page element.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The updated alt text description of the page element.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-update-page-element-alt-text-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UpdatePageElementAltTextRequest
---
