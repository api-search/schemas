---
description: A Bitbucket Cloud commit.
layout: schema
name: Commit
properties_list:
- description: ''
  name: type
  type: string
- description: The commit hash.
  name: hash
  type: string
- description: The commit date.
  name: date
  type: string
- description: The commit author.
  name: author
  type: object
- description: The commit message.
  name: message
  type: string
- description: ''
  name: parents
  type: array
- description: ''
  name: repository
  type: object
provider_name: Bitbucket
provider_slug: bitbucket
schema_file: json-schema/bitbucket-cloud-rest-api-commit-schema.json
slug: bitbucket-cloud-rest-api-commit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/json-schema/bitbucket-cloud-rest-api-commit-schema.json\",\n  \"title\": \"Commit\",\n  \"description\": \"A Bitbucket Cloud commit.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": { \"type\": \"string\" },\n    \"hash\": { \"type\": \"string\", \"description\": \"The commit hash.\" },\n    \"date\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"The commit date.\" },\n    \"author\": { \"type\": \"object\", \"description\": \"The commit author.\", \"properties\": { \"raw\": { \"type\": \"string\" }, \"user\": { \"type\": \"object\" } } },\n    \"message\": { \"type\": \"string\", \"description\": \"The commit message.\" },\n    \"parents\": { \"type\": \"array\", \"items\": { \"type\": \"object\", \"properties\": { \"hash\": { \"type\": \"string\" } } } },\n    \"repository\": { \"\
  type\": \"object\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/json-schema/bitbucket-cloud-rest-api-commit-schema.json
tags:
- Atlassian
- CI/CD
- Code Collaboration
- Code Review
- DevOps
- Git
- Pull Requests
- Repository Hosting
- Version Control
title: Commit
---
