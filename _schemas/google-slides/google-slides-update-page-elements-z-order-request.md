---
description: Updates the Z-order of page elements.
layout: schema
name: UpdatePageElementsZOrderRequest
properties_list:
- description: The object IDs of the page elements to update.
  name: pageElementObjectIds
  type: array
- description: The Z-order operation to apply on the page elements.
  name: operation
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-update-page-elements-z-order-request-schema.json
slug: google-slides-update-page-elements-z-order-request
source_filename: google-slides-update-page-elements-z-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdatePageElementsZOrderRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the Z-order of page elements.\",\n  \"properties\": {\n    \"pageElementObjectIds\": {\n      \"type\": \"array\",\n      \"description\": \"The object IDs of the page elements to update.\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"The Z-order operation to apply on the page elements.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-update-page-elements-z-order-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UpdatePageElementsZOrderRequest
---
