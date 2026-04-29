---
description: A resize job for creating a resized copy of a design
layout: schema
name: ResizeJob
properties_list:
- description: The resize job ID
  name: id
  type: string
- description: The current status of the resize job
  name: status
  type: string
- description: The resize result (present when status is success)
  name: result
  type: object
- description: Error details (present when status is failed)
  name: error
  type: object
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-resize-job-schema.json
slug: canva-connect-resize-job
source_filename: canva-connect-resize-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResizeJob\",\n  \"type\": \"object\",\n  \"description\": \"A resize job for creating a resized copy of a design\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The resize job ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the resize job\"\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"description\": \"The resize result (present when status is success)\"\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Error details (present when status is failed)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-resize-job-schema.json
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
title: ResizeJob
---
