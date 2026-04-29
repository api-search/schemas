---
description: ''
layout: schema
name: TemplateCreateRequest
properties_list:
- description: Template name
  name: name
  type: string
- description: Optional template description
  name: description
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/templatecreaterequest-schema.json
slug: templatecreaterequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/templatecreaterequest-schema.json\",\n  \"title\": \"TemplateCreateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Template name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional template description\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/templatecreaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: TemplateCreateRequest
---
