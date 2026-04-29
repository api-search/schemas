---
description: A user associated with a comment
layout: schema
name: CommentUser
properties_list:
- description: The user ID
  name: id
  type: string
- description: The user display name
  name: display_name
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-comment-user-schema.json
slug: canva-connect-comment-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommentUser\",\n  \"type\": \"object\",\n  \"description\": \"A user associated with a comment\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The user display name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-comment-user-schema.json
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
title: CommentUser
---
