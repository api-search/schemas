---
description: An export job for converting a design to a downloadable format
layout: schema
name: ExportJob
properties_list:
- description: The export job ID
  name: id
  type: string
- description: The current status of the export job
  name: status
  type: string
- description: Download URLs for the exported files (valid for 24 hours). Present only when status is success.
  name: urls
  type: array
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-export-job-schema.json
slug: canva-connect-export-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExportJob\",\n  \"type\": \"object\",\n  \"description\": \"An export job for converting a design to a downloadable format\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The export job ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the export job\"\n    },\n    \"urls\": {\n      \"type\": \"array\",\n      \"description\": \"Download URLs for the exported files (valid for 24 hours). Present only when status is success.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-export-job-schema.json
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
title: ExportJob
---
