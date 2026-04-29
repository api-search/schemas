---
description: PDF export format options
layout: schema
name: PdfExportFormat
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: export_quality
  type: string
- description: Paper size for the PDF
  name: size
  type: string
- description: Page indices to export (exports all pages if omitted)
  name: pages
  type: array
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-pdf-export-format-schema.json
slug: canva-connect-pdf-export-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PdfExportFormat\",\n  \"type\": \"object\",\n  \"description\": \"PDF export format options\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"export_quality\": {\n      \"type\": \"string\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"Paper size for the PDF\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"Page indices to export (exports all pages if omitted)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-pdf-export-format-schema.json
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
title: PdfExportFormat
---
