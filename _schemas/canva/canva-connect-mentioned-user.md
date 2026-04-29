---
description: A user mentioned in a comment
layout: schema
name: MentionedUser
properties_list:
- description: The mentioned user ID
  name: user_id
  type: string
- description: The mentioned user team ID
  name: team_id
  type: string
- description: The mentioned user display name
  name: display_name
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-mentioned-user-schema.json
slug: canva-connect-mentioned-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MentionedUser\",\n  \"type\": \"object\",\n  \"description\": \"A user mentioned in a comment\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"The mentioned user ID\"\n    },\n    \"team_id\": {\n      \"type\": \"string\",\n      \"description\": \"The mentioned user team ID\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The mentioned user display name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-mentioned-user-schema.json
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
title: MentionedUser
---
