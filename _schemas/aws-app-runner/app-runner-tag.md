---
description: Tag schema from AWS App Runner
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: string
- description: ''
  name: Value
  type: string
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-tag-schema.json
slug: app-runner-tag
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\"\n    },\n    \"Value\": {\n      \"type\": \"string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Tag schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-tag-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: Tag
---
