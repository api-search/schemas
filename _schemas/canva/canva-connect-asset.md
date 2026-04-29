---
description: A Canva asset (image or video)
layout: schema
name: Asset
properties_list:
- description: The asset ID
  name: id
  type: string
- description: The asset type
  name: type
  type: string
- description: The asset name
  name: name
  type: string
- description: User-facing tags for the asset
  name: tags
  type: array
- description: Unix timestamp in seconds when the asset was created
  name: created_at
  type: integer
- description: Unix timestamp in seconds when the asset was last updated
  name: updated_at
  type: integer
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-asset-schema.json
slug: canva-connect-asset
source_filename: canva-connect-asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Asset\",\n  \"type\": \"object\",\n  \"description\": \"A Canva asset (image or video)\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The asset type\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The asset name\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"User-facing tags for the asset\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the asset was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the asset was last updated\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-asset-schema.json
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
title: Asset
---
