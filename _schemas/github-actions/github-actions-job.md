---
description: ''
layout: schema
name: Job
properties_list:
- description: The id of the job.
  name: id
  type: integer
- description: The id of the associated workflow run.
  name: run_id
  type: integer
- description: ''
  name: run_url
  type: string
- description: ''
  name: run_attempt
  type: integer
- description: ''
  name: node_id
  type: string
- description: ''
  name: head_sha
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: conclusion
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: started_at
  type: string
- description: ''
  name: completed_at
  type: string
- description: The name of the job.
  name: name
  type: string
- description: ''
  name: steps
  type: array
- description: ''
  name: labels
  type: array
- description: ''
  name: runner_id
  type: integer
- description: ''
  name: runner_name
  type: string
- description: ''
  name: runner_group_id
  type: integer
- description: ''
  name: runner_group_name
  type: string
- description: ''
  name: workflow_name
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-job-schema.json
slug: github-actions-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The id of the job.\"\n    },\n    \"run_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The id of the associated workflow run.\"\n    },\n    \"run_url\": {\n      \"type\": \"string\"\n    },\n    \"run_attempt\": {\n      \"type\": \"integer\"\n    },\n    \"node_id\": {\n      \"type\": \"string\"\n    },\n    \"head_sha\": {\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    },\n    \"html_url\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"conclusion\": {\n      \"type\": \"string\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"started_at\": {\n      \"type\": \"string\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\"\n \
  \   },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job.\"\n    },\n    \"steps\": {\n      \"type\": \"array\"\n    },\n    \"labels\": {\n      \"type\": \"array\"\n    },\n    \"runner_id\": {\n      \"type\": \"integer\"\n    },\n    \"runner_name\": {\n      \"type\": \"string\"\n    },\n    \"runner_group_id\": {\n      \"type\": \"integer\"\n    },\n    \"runner_group_name\": {\n      \"type\": \"string\"\n    },\n    \"workflow_name\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-job-schema.json
tags: []
title: Job
---
