---
description: Request body for creating a design resize job
layout: schema
name: CreateResizeJobRequest
properties_list:
- description: The design ID to resize
  name: design_id
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-create-resize-job-request-schema.json
slug: canva-connect-create-resize-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateResizeJobRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a design resize job\",\n  \"properties\": {\n    \"design_id\": {\n      \"type\": \"string\",\n      \"description\": \"The design ID to resize\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-create-resize-job-request-schema.json
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
title: CreateResizeJobRequest
---
