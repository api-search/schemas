---
description: A Bitbucket Cloud pull request.
layout: schema
name: Pullrequest
properties_list:
- description: ''
  name: type
  type: string
- description: The pull request ID.
  name: id
  type: integer
- description: The pull request title.
  name: title
  type: string
- description: The pull request description.
  name: description
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: created_on
  type: string
- description: ''
  name: updated_on
  type: string
- description: ''
  name: close_source_branch
  type: boolean
- description: The author of the pull request.
  name: author
  type: object
- description: The source branch.
  name: source
  type: object
- description: The destination branch.
  name: destination
  type: object
- description: ''
  name: merge_commit
  type: object
- description: ''
  name: comment_count
  type: integer
- description: ''
  name: task_count
  type: integer
- description: ''
  name: reviewers
  type: array
- description: ''
  name: participants
  type: array
provider_name: Bitbucket
provider_slug: bitbucket
schema_file: json-schema/bitbucket-cloud-rest-api-pullrequest-schema.json
slug: bitbucket-cloud-rest-api-pullrequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/json-schema/bitbucket-cloud-rest-api-pullrequest-schema.json\",\n  \"title\": \"Pullrequest\",\n  \"description\": \"A Bitbucket Cloud pull request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": { \"type\": \"string\" },\n    \"id\": { \"type\": \"integer\", \"description\": \"The pull request ID.\" },\n    \"title\": { \"type\": \"string\", \"description\": \"The pull request title.\" },\n    \"description\": { \"type\": \"string\", \"description\": \"The pull request description.\" },\n    \"state\": { \"type\": \"string\", \"enum\": [\"OPEN\", \"MERGED\", \"DECLINED\", \"SUPERSEDED\"] },\n    \"created_on\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"updated_on\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"close_source_branch\": { \"type\": \"boolean\" },\n    \"author\"\
  : { \"type\": \"object\", \"description\": \"The author of the pull request.\" },\n    \"source\": { \"type\": \"object\", \"description\": \"The source branch.\", \"properties\": { \"branch\": { \"type\": \"object\", \"properties\": { \"name\": { \"type\": \"string\" } } }, \"repository\": { \"type\": \"object\" } } },\n    \"destination\": { \"type\": \"object\", \"description\": \"The destination branch.\", \"properties\": { \"branch\": { \"type\": \"object\", \"properties\": { \"name\": { \"type\": \"string\" } } }, \"repository\": { \"type\": \"object\" } } },\n    \"merge_commit\": { \"type\": \"object\", \"properties\": { \"hash\": { \"type\": \"string\" } } },\n    \"comment_count\": { \"type\": \"integer\" },\n    \"task_count\": { \"type\": \"integer\" },\n    \"reviewers\": { \"type\": \"array\", \"items\": { \"type\": \"object\" } },\n    \"participants\": { \"type\": \"array\", \"items\": { \"type\": \"object\" } }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/json-schema/bitbucket-cloud-rest-api-pullrequest-schema.json
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
title: Pullrequest
---
