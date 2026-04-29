---
description: ''
layout: schema
name: ProjectConstructionRequest
properties_list:
- description: ''
  name: project
  type: object
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/projectconstructionrequest-schema.json
slug: projectconstructionrequest
source_filename: projectconstructionrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/projectconstructionrequest-schema.json\",\n  \"title\": \"ProjectConstructionRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"project\"\n  ],\n  \"properties\": {\n    \"project\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the new project being constructed\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Optional description for the new project\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/projectconstructionrequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ProjectConstructionRequest
---
