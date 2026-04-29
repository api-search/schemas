---
description: A Bitbucket Pipelines CI/CD pipeline.
layout: schema
name: Pipeline
properties_list:
- description: ''
  name: type
  type: string
- description: The pipeline UUID.
  name: uuid
  type: string
- description: The build number.
  name: build_number
  type: integer
- description: The user who triggered the pipeline.
  name: creator
  type: object
- description: The repository.
  name: repository
  type: object
- description: The pipeline target (branch, tag, etc.).
  name: target
  type: object
- description: The pipeline state.
  name: state
  type: object
- description: ''
  name: created_on
  type: string
- description: ''
  name: completed_on
  type: string
- description: ''
  name: build_seconds_used
  type: integer
provider_name: Bitbucket
provider_slug: bitbucket
schema_file: json-schema/bitbucket-cloud-rest-api-pipeline-schema.json
slug: bitbucket-cloud-rest-api-pipeline
source_filename: bitbucket-cloud-rest-api-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/json-schema/bitbucket-cloud-rest-api-pipeline-schema.json\",\n  \"title\": \"Pipeline\",\n  \"description\": \"A Bitbucket Pipelines CI/CD pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": { \"type\": \"string\" },\n    \"uuid\": { \"type\": \"string\", \"description\": \"The pipeline UUID.\" },\n    \"build_number\": { \"type\": \"integer\", \"description\": \"The build number.\" },\n    \"creator\": { \"type\": \"object\", \"description\": \"The user who triggered the pipeline.\" },\n    \"repository\": { \"type\": \"object\", \"description\": \"The repository.\" },\n    \"target\": { \"type\": \"object\", \"description\": \"The pipeline target (branch, tag, etc.).\" },\n    \"state\": { \"type\": \"object\", \"description\": \"The pipeline state.\", \"properties\": { \"name\": { \"type\": \"string\"\
  , \"enum\": [\"PENDING\", \"IN_PROGRESS\", \"COMPLETED\", \"HALTED\", \"PAUSED\"] } } },\n    \"created_on\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"completed_on\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"build_seconds_used\": { \"type\": \"integer\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/json-schema/bitbucket-cloud-rest-api-pipeline-schema.json
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
title: Pipeline
---
