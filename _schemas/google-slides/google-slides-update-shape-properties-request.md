---
description: Update the properties of a Shape.
layout: schema
name: UpdateShapePropertiesRequest
properties_list:
- description: The object ID of the shape.
  name: objectId
  type: string
- description: The fields that should be updated. At least one field must be specified. Uses Google's FieldMask format.
  name: fields
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-update-shape-properties-request-schema.json
slug: google-slides-update-shape-properties-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateShapePropertiesRequest\",\n  \"type\": \"object\",\n  \"description\": \"Update the properties of a Shape.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the shape.\"\n    },\n    \"fields\": {\n      \"type\": \"string\",\n      \"description\": \"The fields that should be updated. At least one field must be specified. Uses Google's FieldMask format.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-update-shape-properties-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UpdateShapePropertiesRequest
---
