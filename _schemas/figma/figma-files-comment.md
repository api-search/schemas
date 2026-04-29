---
description: A comment or reply left by a user.
layout: schema
name: Comment
properties_list:
- description: Unique identifier for comment.
  name: id
  type: string
- description: The file in which the comment lives.
  name: fileKey
  type: string
- description: If present, the id of the comment to which this is the reply.
  name: parentId
  type: string
- description: The UTC ISO 8601 time at which the comment was left.
  name: createdAt
  type: string
- description: If set, the UTC ISO 8601 time the comment was resolved.
  name: resolvedAt
  type: '[''string'', ''null'']'
- description: The content of the comment.
  name: message
  type: string
- description: The number displayed with the comment in the UI.
  name: orderId
  type: '[''string'', ''null'']'
- description: An array of reactions to the comment.
  name: reactions
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-files-comment-schema.json
slug: figma-files-comment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Comment\",\n  \"type\": \"object\",\n  \"description\": \"A comment or reply left by a user.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for comment.\"\n    },\n    \"fileKey\": {\n      \"type\": \"string\",\n      \"description\": \"The file in which the comment lives.\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"If present, the id of the comment to which this is the reply.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time at which the comment was left.\"\n    },\n    \"resolvedAt\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"If set, the UTC ISO 8601 time the comment was resolved.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the comment.\"\n   \
  \ },\n    \"orderId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The number displayed with the comment in the UI.\"\n    },\n    \"reactions\": {\n      \"type\": \"array\",\n      \"description\": \"An array of reactions to the comment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-files-comment-schema.json
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
