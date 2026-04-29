---
description: A Canva folder
layout: schema
name: Folder
properties_list:
- description: The folder ID
  name: id
  type: string
- description: The folder name
  name: name
  type: string
- description: Unix timestamp in seconds when the folder was created
  name: created_at
  type: integer
- description: Unix timestamp in seconds when the folder was last updated
  name: updated_at
  type: integer
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-folder-schema.json
slug: canva-connect-folder
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Folder\",\n  \"type\": \"object\",\n  \"description\": \"A Canva folder\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The folder ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The folder name\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the folder was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the folder was last updated\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-folder-schema.json
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
title: Folder
---
