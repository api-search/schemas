---
description: ''
layout: schema
name: CommentCreateRequest
properties_list:
- description: The ID of the blog post to comment on.
  name: blogPostId
  type: string
- description: The ID of the page to comment on.
  name: pageId
  type: string
- description: The ID of the parent comment for replies.
  name: parentCommentId
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-comment-create-request-schema.json
slug: confluence-cloud-v2-comment-create-request
source_filename: confluence-cloud-v2-comment-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommentCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"blogPostId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the blog post to comment on.\"\n    },\n    \"pageId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the page to comment on.\"\n    },\n    \"parentCommentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the parent comment for replies.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-comment-create-request-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: CommentCreateRequest
---
