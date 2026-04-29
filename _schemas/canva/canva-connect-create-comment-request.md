---
description: Request body for creating a comment
layout: schema
name: CreateCommentRequest
properties_list:
- description: Comment text (1-2048 characters). Mention users with [user_id:team_id] format.
  name: message
  type: string
- description: User ID to assign the comment to
  name: assignee_id
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-create-comment-request-schema.json
slug: canva-connect-create-comment-request
source_filename: canva-connect-create-comment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCommentRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a comment\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Comment text (1-2048 characters). Mention users with [user_id:team_id] format.\"\n    },\n    \"assignee_id\": {\n      \"type\": \"string\",\n      \"description\": \"User ID to assign the comment to\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-create-comment-request-schema.json
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
title: CreateCommentRequest
---
