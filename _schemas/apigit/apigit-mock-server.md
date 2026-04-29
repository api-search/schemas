---
description: An APIGit dynamic mock server instance.
layout: schema
name: MockServer
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: repoId
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: status
  type: string
provider_name: APIGit
provider_slug: apigit
schema_file: json-schema/apigit-mock-server-schema.json
slug: apigit-mock-server
source_filename: apigit-mock-server-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/json-schema/apigit-mock-server-schema.json\",\n  \"title\": \"MockServer\",\n  \"description\": \"An APIGit dynamic mock server instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"mock-001\"\n    },\n    \"repoId\": {\n      \"type\": \"string\",\n      \"example\": \"repo-001\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"running\",\n        \"stopped\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/json-schema/apigit-mock-server-schema.json
tags:
- API Design
- API Lifecycle
- Documentation
- Git
- Governance
- Mocking
- Platform
- Testing
title: MockServer
---
