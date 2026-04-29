---
description: Error details for a failed export job
layout: schema
name: ExportError
properties_list:
- description: Error code indicating the reason for failure
  name: code
  type: string
- description: Human-readable error message
  name: message
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-export-error-schema.json
slug: canva-connect-export-error
source_filename: canva-connect-export-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExportError\",\n  \"type\": \"object\",\n  \"description\": \"Error details for a failed export job\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code indicating the reason for failure\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-export-error-schema.json
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
title: ExportError
---
