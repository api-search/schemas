---
description: A comment or reply left by a user on a Figma file. Comments can be pinned to specific locations on the canvas.
layout: schema
name: Comment
properties_list:
- description: Unique identifier for the comment.
  name: id
  type: string
- description: The key of the file the comment belongs to.
  name: file_key
  type: string
- description: If present, the ID of the comment to which this is a reply.
  name: parent_id
  type: '[''string'', ''null'']'
- description: The UTC ISO 8601 time at which the comment was left.
  name: created_at
  type: string
- description: If set, the UTC ISO 8601 time the comment was resolved.
  name: resolved_at
  type: '[''string'', ''null'']'
- description: The content of the comment.
  name: message
  type: string
- description: Only set for top-level comments. The number displayed with the comment in the UI.
  name: order_id
  type: '[''string'', ''null'']'
- description: An array of emoji reactions to the comment.
  name: reactions
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-comment-schema.json
slug: figma-rest-comment
source_filename: figma-rest-comment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Comment\",\n  \"type\": \"object\",\n  \"description\": \"A comment or reply left by a user on a Figma file. Comments can be pinned to specific locations on the canvas.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the comment.\"\n    },\n    \"file_key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the file the comment belongs to.\"\n    },\n    \"parent_id\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"If present, the ID of the comment to which this is a reply.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time at which the comment was left.\"\n    },\n    \"resolved_at\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"If set, the UTC ISO 8601 time the comment was resolved.\"\n    },\n    \"message\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The content of the comment.\"\n    },\n    \"order_id\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Only set for top-level comments. The number displayed with the comment in the UI.\"\n    },\n    \"reactions\": {\n      \"type\": \"array\",\n      \"description\": \"An array of emoji reactions to the comment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-comment-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: Comment
---
