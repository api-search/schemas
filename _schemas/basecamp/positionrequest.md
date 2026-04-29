---
description: ''
layout: schema
name: PositionRequest
properties_list:
- description: New position within the list (1-indexed)
  name: position
  type: integer
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/positionrequest-schema.json
slug: positionrequest
source_filename: positionrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/positionrequest-schema.json\",\n  \"title\": \"PositionRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"position\"\n  ],\n  \"properties\": {\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\": \"New position within the list (1-indexed)\",\n      \"minimum\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/positionrequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: PositionRequest
---
