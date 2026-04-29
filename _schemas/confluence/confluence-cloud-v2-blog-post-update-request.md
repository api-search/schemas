---
description: ''
layout: schema
name: BlogPostUpdateRequest
properties_list:
- description: The ID of the blog post being updated.
  name: id
  type: string
- description: The status of the blog post.
  name: status
  type: string
- description: The new title of the blog post.
  name: title
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-blog-post-update-request-schema.json
slug: confluence-cloud-v2-blog-post-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlogPostUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the blog post being updated.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the blog post.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The new title of the blog post.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-blog-post-update-request-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: BlogPostUpdateRequest
---
