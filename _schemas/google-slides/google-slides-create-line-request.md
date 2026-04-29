---
description: Creates a line.
layout: schema
name: CreateLineRequest
properties_list:
- description: A user-supplied object ID.
  name: objectId
  type: string
- description: The category of the line to be created.
  name: lineCategory
  type: string
- description: The category of the line to be created (preferred over lineCategory).
  name: category
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-create-line-request-schema.json
slug: google-slides-create-line-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateLineRequest\",\n  \"type\": \"object\",\n  \"description\": \"Creates a line.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"A user-supplied object ID.\"\n    },\n    \"lineCategory\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the line to be created.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the line to be created (preferred over lineCategory).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-create-line-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: CreateLineRequest
---
