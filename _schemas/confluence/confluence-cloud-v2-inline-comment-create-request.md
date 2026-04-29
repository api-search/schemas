---
description: ''
layout: schema
name: InlineCommentCreateRequest
properties_list:
- description: The ID of the blog post to add an inline comment on.
  name: blogPostId
  type: string
- description: The ID of the page to add an inline comment on.
  name: pageId
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-inline-comment-create-request-schema.json
slug: confluence-cloud-v2-inline-comment-create-request
source_filename: confluence-cloud-v2-inline-comment-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InlineCommentCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"blogPostId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the blog post to add an inline comment on.\"\n    },\n    \"pageId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the page to add an inline comment on.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-inline-comment-create-request-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: InlineCommentCreateRequest
---
