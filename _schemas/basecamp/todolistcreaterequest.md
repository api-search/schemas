---
description: ''
layout: schema
name: TodoListCreateRequest
properties_list:
- description: To-do list name
  name: name
  type: string
- description: Optional description with supported HTML formatting
  name: description
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/todolistcreaterequest-schema.json
slug: todolistcreaterequest
source_filename: todolistcreaterequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/todolistcreaterequest-schema.json\",\n  \"title\": \"TodoListCreateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"To-do list name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description with supported HTML formatting\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/todolistcreaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: TodoListCreateRequest
---
