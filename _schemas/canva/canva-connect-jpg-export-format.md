---
description: JPG export format options
layout: schema
name: JpgExportFormat
properties_list:
- description: ''
  name: type
  type: string
- description: JPG compression quality (1-100)
  name: quality
  type: integer
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
schema_file: json-schema/canva-connect-jpg-export-format-schema.json
slug: canva-connect-jpg-export-format
source_filename: canva-connect-jpg-export-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JpgExportFormat\",\n  \"type\": \"object\",\n  \"description\": \"JPG export format options\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"quality\": {\n      \"type\": \"integer\",\n      \"description\": \"JPG compression quality (1-100)\"\n    },\n    \"export_quality\": {\n      \"type\": \"string\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Output width in pixels\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Output height in pixels\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"Page indices to export\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-jpg-export-format-schema.json
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
title: JpgExportFormat
---
