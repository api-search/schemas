---
description: The authenticated user and their team
layout: schema
name: TeamUser
properties_list:
- description: The user ID
  name: user_id
  type: string
- description: The team ID
  name: team_id
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-team-user-schema.json
slug: canva-connect-team-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TeamUser\",\n  \"type\": \"object\",\n  \"description\": \"The authenticated user and their team\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID\"\n    },\n    \"team_id\": {\n      \"type\": \"string\",\n      \"description\": \"The team ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-team-user-schema.json
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
title: TeamUser
---
