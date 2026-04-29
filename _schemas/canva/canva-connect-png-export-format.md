---
description: PNG export format options
layout: schema
name: PngExportFormat
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
- description: Whether to use lossless compression
  name: lossless
  type: boolean
- description: Whether to use a transparent background
  name: transparent_background
  type: boolean
- description: Whether to export all pages as a single image
  name: as_single_image
  type: boolean
- description: Page indices to export
  name: pages
  type: array
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-png-export-format-schema.json
slug: canva-connect-png-export-format
source_filename: canva-connect-png-export-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PngExportFormat\",\n  \"type\": \"object\",\n  \"description\": \"PNG export format options\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"export_quality\": {\n      \"type\": \"string\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Output width in pixels\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Output height in pixels\"\n    },\n    \"lossless\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use lossless compression\"\n    },\n    \"transparent_background\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use a transparent background\"\n    },\n    \"as_single_image\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to export all pages as a single image\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n    \
  \  \"description\": \"Page indices to export\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-png-export-format-schema.json
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
title: PngExportFormat
---
