---
description: PowerPoint export format options
layout: schema
name: PptxExportFormat
properties_list:
- description: ''
  name: type
  type: string
- description: Page indices to export
  name: pages
  type: array
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-pptx-export-format-schema.json
slug: canva-connect-pptx-export-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PptxExportFormat\",\n  \"type\": \"object\",\n  \"description\": \"PowerPoint export format options\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"Page indices to export\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-pptx-export-format-schema.json
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
title: PptxExportFormat
---
