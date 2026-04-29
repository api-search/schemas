---
description: The owner of a resource
layout: schema
name: Owner
properties_list:
- description: The user ID of the owner
  name: user_id
  type: string
- description: The team ID of the owner
  name: team_id
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-owner-schema.json
slug: canva-connect-owner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Owner\",\n  \"type\": \"object\",\n  \"description\": \"The owner of a resource\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the owner\"\n    },\n    \"team_id\": {\n      \"type\": \"string\",\n      \"description\": \"The team ID of the owner\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-owner-schema.json
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
title: Owner
---
