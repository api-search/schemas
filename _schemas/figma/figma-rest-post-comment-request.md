---
description: Request body for posting a new comment.
layout: schema
name: PostCommentRequest
properties_list:
- description: The text content of the comment.
  name: message
  type: string
- description: The comment to reply to, if any. This must be a root comment. Creating a reply to a reply is not supported.
  name: comment_id
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-post-comment-request-schema.json
slug: figma-rest-post-comment-request
source_filename: figma-rest-post-comment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PostCommentRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for posting a new comment.\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The text content of the comment.\"\n    },\n    \"comment_id\": {\n      \"type\": \"string\",\n      \"description\": \"The comment to reply to, if any. This must be a root comment. Creating a reply to a reply is not supported.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-post-comment-request-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: PostCommentRequest
---
