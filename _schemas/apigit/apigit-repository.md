---
description: An APIGit API repository.
layout: schema
name: Repository
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: visibility
  type: string
provider_name: APIGit
provider_slug: apigit
schema_file: json-schema/apigit-repository-schema.json
slug: apigit-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/json-schema/apigit-repository-schema.json\",\n  \"title\": \"Repository\",\n  \"description\": \"An APIGit API repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"repo-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"my-api\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"public\",\n        \"private\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/json-schema/apigit-repository-schema.json
tags:
- API Design
- API Lifecycle
- Documentation
- Git
- Governance
- Mocking
- Platform
- Testing
title: Repository
---
