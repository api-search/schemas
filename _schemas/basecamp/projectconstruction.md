---
description: ''
layout: schema
name: ProjectConstruction
properties_list:
- description: Project construction job ID
  name: id
  type: integer
- description: Construction status
  name: status
  type: string
- description: API URL to poll for this construction job
  name: url
  type: string
- description: The resulting project once construction is completed
  name: project
  type: object
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/projectconstruction-schema.json
slug: projectconstruction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/projectconstruction-schema.json\",\n  \"title\": \"ProjectConstruction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Project construction job ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Construction status\",\n      \"enum\": [\n        \"pending\",\n        \"completed\"\n      ]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL to poll for this construction job\"\n    },\n    \"project\": {\n      \"$ref\": \"#/components/schemas/Project\",\n      \"description\": \"The resulting project once construction is completed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/projectconstruction-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ProjectConstruction
---
