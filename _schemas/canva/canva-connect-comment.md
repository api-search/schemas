---
description: A comment on a design
layout: schema
name: Comment
properties_list:
- description: The comment type
  name: type
  type: string
- description: The comment ID
  name: id
  type: string
- description: The comment text. User mentions use the format [user_id:team_id].
  name: message
  type: string
- description: Unix timestamp in seconds when the comment was created
  name: created_at
  type: integer
- description: Unix timestamp in seconds when the comment was last updated
  name: updated_at
  type: integer
- description: Dictionary of mentioned users, keyed by their mention identifier
  name: mentions
  type: object
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-comment-schema.json
slug: canva-connect-comment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Comment\",\n  \"type\": \"object\",\n  \"description\": \"A comment on a design\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The comment type\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The comment ID\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The comment text. User mentions use the format [user_id:team_id].\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the comment was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the comment was last updated\"\n    },\n    \"mentions\": {\n      \"type\": \"object\",\n      \"description\": \"Dictionary of mentioned users, keyed by their mention identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-comment-schema.json
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
title: Comment
---
