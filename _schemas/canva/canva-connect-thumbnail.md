---
description: A thumbnail image for a resource (URL expires in 15 minutes)
layout: schema
name: Thumbnail
properties_list:
- description: Thumbnail width in pixels
  name: width
  type: integer
- description: Thumbnail height in pixels
  name: height
  type: integer
- description: Thumbnail URL (expires in 15 minutes)
  name: url
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-thumbnail-schema.json
slug: canva-connect-thumbnail
source_filename: canva-connect-thumbnail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Thumbnail\",\n  \"type\": \"object\",\n  \"description\": \"A thumbnail image for a resource (URL expires in 15 minutes)\",\n  \"properties\": {\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Thumbnail width in pixels\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Thumbnail height in pixels\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Thumbnail URL (expires in 15 minutes)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-thumbnail-schema.json
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
title: Thumbnail
---
