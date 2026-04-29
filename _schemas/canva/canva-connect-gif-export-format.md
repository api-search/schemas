---
description: GIF export format options
layout: schema
name: GifExportFormat
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: export_quality
  type: string
- description: Output width in pixels
  name: width
  type: integer
- description: Output height in pixels
  name: height
  type: integer
- description: Page indices to export
  name: pages
  type: array
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-gif-export-format-schema.json
slug: canva-connect-gif-export-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GifExportFormat\",\n  \"type\": \"object\",\n  \"description\": \"GIF export format options\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"export_quality\": {\n      \"type\": \"string\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Output width in pixels\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Output height in pixels\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"Page indices to export\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-gif-export-format-schema.json
tags:
- Apps
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
title: GifExportFormat
---
