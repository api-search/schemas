---
description: Updates the transform of a page element.
layout: schema
name: UpdatePageElementTransformRequest
properties_list:
- description: The object ID of the page element to update.
  name: objectId
  type: string
- description: The apply mode of the transform update.
  name: applyMode
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-update-page-element-transform-request-schema.json
slug: google-slides-update-page-element-transform-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdatePageElementTransformRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the transform of a page element.\\n\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the page element to update.\"\n    },\n    \"applyMode\": {\n      \"type\": \"string\",\n      \"description\": \"The apply mode of the transform update.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-update-page-element-transform-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UpdatePageElementTransformRequest
---
