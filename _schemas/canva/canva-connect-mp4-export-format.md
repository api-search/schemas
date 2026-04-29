---
description: MP4 video export format options
layout: schema
name: Mp4ExportFormat
properties_list:
- description: ''
  name: type
  type: string
- description: Video quality and orientation
  name: quality
  type: string
- description: ''
  name: export_quality
  type: string
- description: Page indices to export
  name: pages
  type: array
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-mp4-export-format-schema.json
slug: canva-connect-mp4-export-format
source_filename: canva-connect-mp4-export-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Mp4ExportFormat\",\n  \"type\": \"object\",\n  \"description\": \"MP4 video export format options\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"quality\": {\n      \"type\": \"string\",\n      \"description\": \"Video quality and orientation\"\n    },\n    \"export_quality\": {\n      \"type\": \"string\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"Page indices to export\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-mp4-export-format-schema.json
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
title: Mp4ExportFormat
---
