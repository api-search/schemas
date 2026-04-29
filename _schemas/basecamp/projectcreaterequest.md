---
description: ''
layout: schema
name: ProjectCreateRequest
properties_list:
- description: Name for the new project
  name: name
  type: string
- description: Optional description of the project
  name: description
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/projectcreaterequest-schema.json
slug: projectcreaterequest
source_filename: projectcreaterequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/projectcreaterequest-schema.json\",\n  \"title\": \"ProjectCreateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the new project\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the project\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/projectcreaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ProjectCreateRequest
---
