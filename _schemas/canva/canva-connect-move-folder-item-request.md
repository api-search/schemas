---
description: Request body for moving an item to a folder
layout: schema
name: MoveFolderItemRequest
properties_list:
- description: The ID of the item to move
  name: item_id
  type: string
- description: The type of item to move
  name: item_type
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-move-folder-item-request-schema.json
slug: canva-connect-move-folder-item-request
source_filename: canva-connect-move-folder-item-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MoveFolderItemRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for moving an item to a folder\",\n  \"properties\": {\n    \"item_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the item to move\"\n    },\n    \"item_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of item to move\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-move-folder-item-request-schema.json
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
title: MoveFolderItemRequest
---
