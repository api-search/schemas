---
description: Represents a Confluence blog post.
layout: schema
name: BlogPost
properties_list:
- description: The unique identifier of the blog post.
  name: id
  type: string
- description: The current status of the blog post.
  name: status
  type: string
- description: The title of the blog post.
  name: title
  type: string
- description: The ID of the space this blog post belongs to.
  name: spaceId
  type: string
- description: The Atlassian account ID of the blog post author.
  name: authorId
  type: string
- description: The ISO 8601 timestamp when the blog post was created.
  name: createdAt
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-blog-post-schema.json
slug: confluence-cloud-v2-blog-post
source_filename: confluence-cloud-v2-blog-post-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlogPost\",\n  \"type\": \"object\",\n  \"description\": \"Represents a Confluence blog post.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the blog post.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the blog post.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the blog post.\"\n    },\n    \"spaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the space this blog post belongs to.\"\n    },\n    \"authorId\": {\n      \"type\": \"string\",\n      \"description\": \"The Atlassian account ID of the blog post author.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 8601 timestamp when the blog post was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-blog-post-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: BlogPost
---
