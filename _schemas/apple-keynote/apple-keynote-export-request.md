---
description: Request body for exporting an Apple Keynote presentation
layout: schema
name: ExportRequest
properties_list:
- description: Export format
  name: format
  type: string
- description: Whether to include presenter notes
  name: includeNotes
  type: boolean
- description: Slide range to export (e.g. 1-5,8)
  name: slideRange
  type: string
provider_name: Apple Keynote
provider_slug: apple-keynote
schema_file: json-schema/apple-keynote-export-request-schema.json
slug: apple-keynote-export-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apple-keynote/refs/heads/main/json-schema/apple-keynote-export-request-schema.json\",\n  \"title\": \"ExportRequest\",\n  \"description\": \"Request body for exporting an Apple Keynote presentation\",\n  \"type\": \"object\",\n  \"required\": [\n    \"format\"\n  ],\n  \"properties\": {\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pdf\",\n        \"pptx\",\n        \"key\",\n        \"html\",\n        \"images\"\n      ],\n      \"description\": \"Export format\",\n      \"example\": \"pdf\"\n    },\n    \"includeNotes\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include presenter notes\",\n      \"example\": true\n    },\n    \"slideRange\": {\n      \"type\": \"string\",\n      \"description\": \"Slide range to export (e.g. 1-5,8)\",\n      \"example\": \"1-24\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple-keynote/refs/heads/main/json-schema/apple-keynote-export-request-schema.json
tags:
- Apple
- Design
- iWork
- Presentations
- Productivity
- Slides
title: ExportRequest
---
