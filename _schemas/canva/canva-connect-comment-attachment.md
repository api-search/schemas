---
description: The object a comment is attached to
layout: schema
name: CommentAttachment
properties_list:
- description: The attachment type
  name: type
  type: string
- description: The design ID the comment is attached to
  name: design_id
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-comment-attachment-schema.json
slug: canva-connect-comment-attachment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommentAttachment\",\n  \"type\": \"object\",\n  \"description\": \"The object a comment is attached to\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The attachment type\"\n    },\n    \"design_id\": {\n      \"type\": \"string\",\n      \"description\": \"The design ID the comment is attached to\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-comment-attachment-schema.json
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
title: CommentAttachment
---
