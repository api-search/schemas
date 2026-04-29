---
description: ''
layout: schema
name: DocumentCreateRequest
properties_list:
- description: Document title
  name: title
  type: string
- description: Document body in HTML format
  name: content
  type: string
- description: Set to "active" to publish immediately
  name: status
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/documentcreaterequest-schema.json
slug: documentcreaterequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/documentcreaterequest-schema.json\",\n  \"title\": \"DocumentCreateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"title\",\n    \"content\"\n  ],\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Document title\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Document body in HTML format\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Set to \\\"active\\\" to publish immediately\",\n      \"enum\": [\n        \"active\",\n        \"draft\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/documentcreaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: DocumentCreateRequest
---
