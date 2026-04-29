---
description: ''
layout: schema
name: BlogPostCreateRequest
properties_list:
- description: The ID of the space to create the blog post in.
  name: spaceId
  type: string
- description: The status of the blog post.
  name: status
  type: string
- description: The title of the blog post.
  name: title
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-blog-post-create-request-schema.json
slug: confluence-cloud-v2-blog-post-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlogPostCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the space to create the blog post in.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the blog post.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the blog post.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-blog-post-create-request-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: BlogPostCreateRequest
---
