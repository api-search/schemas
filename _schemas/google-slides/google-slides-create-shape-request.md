---
description: Creates a new shape.
layout: schema
name: CreateShapeRequest
properties_list:
- description: A user-supplied object ID.
  name: objectId
  type: string
- description: The shape type.
  name: shapeType
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-create-shape-request-schema.json
slug: google-slides-create-shape-request
source_filename: google-slides-create-shape-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateShapeRequest\",\n  \"type\": \"object\",\n  \"description\": \"Creates a new shape.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"A user-supplied object ID.\"\n    },\n    \"shapeType\": {\n      \"type\": \"string\",\n      \"description\": \"The shape type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-create-shape-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: CreateShapeRequest
---
