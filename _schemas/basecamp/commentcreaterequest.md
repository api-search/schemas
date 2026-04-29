---
description: ''
layout: schema
name: CommentCreateRequest
properties_list:
- description: Comment body in HTML format
  name: content
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/commentcreaterequest-schema.json
slug: commentcreaterequest
source_filename: commentcreaterequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/commentcreaterequest-schema.json\",\n  \"title\": \"CommentCreateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"content\"\n  ],\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Comment body in HTML format\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/commentcreaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: CommentCreateRequest
---
