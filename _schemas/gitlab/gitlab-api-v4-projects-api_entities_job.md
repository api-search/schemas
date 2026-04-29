---
description: API_Entities_Job model
layout: schema
name: API_Entities_Job
properties_list:
- description: The ID of the job
  name: id
  type: integer
- description: The name of the job
  name: name
  type: string
- description: The current status of the job
  name: status
  type: string
- description: The stage of the job in the CI/CD pipeline
  name: stage
  type: string
- description: The creation time of the job
  name: created_at
  type: string
- description: The start time of the job
  name: started_at
  type: string
- description: The finish time of the job
  name: finished_at
  type: string
- description: ''
  name: commit
  type: object
- description: Indicates if the job is archived
  name: archived
  type: boolean
- description: Indicates if the job is allowed to fail
  name: allow_failure
  type: boolean
- description: The time when the job was erased, if applicable
  name: erased_at
  type: string
- description: The duration of the job in seconds
  name: duration
  type: integer
- description: The duration the job was queued before execution, in seconds
  name: queued_duration
  type: number
- description: The reference for the job
  name: ref
  type: string
- description: The artifacts produced by the job
  name: artifacts
  type: array
- description: Indicates if the job is tagged
  name: tag
  type: boolean
- description: The URL for accessing the job in the web interface
  name: web_url
  type: string
- description: ''
  name: project
  type: object
- description: The user that started the job
  name: user
  type: object
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-projects-api_entities_job-schema.json
slug: gitlab-api-v4-projects-api_entities_job
source_filename: gitlab-api-v4-projects-api_entities_job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-projects-api_entities_job-schema.json\",\n  \"title\": \"API_Entities_Job\",\n  \"description\": \"API_Entities_Job model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the job\",\n      \"example\": 42\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job\",\n      \"example\": \"Example Project\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the job\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"stage\": {\n      \"type\": \"string\",\n      \"description\": \"The stage of the job in the CI/CD pipeline\",\n      \"example\": \"example_value\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"example\": \"2016-01-11T10:13:33.506Z\",\n      \"description\": \"The creation time of the job\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2016-01-11T10:13:33.506Z\",\n      \"description\": \"The start time of the job\"\n    },\n    \"finished_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2016-01-11T10:13:33.506Z\",\n      \"description\": \"The finish time of the job\"\n    },\n    \"commit\": {\n      \"$ref\": \"#/components/schemas/API_Entities_Commit\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the job is archived\",\n      \"example\": true\n    },\n    \"allow_failure\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the job is allowed to fail\",\n      \"example\": true\n    },\n    \"erased_at\": {\n      \"type\": \"string\",\n     \
  \ \"format\": \"date-time\",\n      \"example\": \"2016-01-11T10:13:33.506Z\",\n      \"description\": \"The time when the job was erased, if applicable\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"The duration of the job in seconds\",\n      \"example\": 42\n    },\n    \"queued_duration\": {\n      \"type\": \"number\",\n      \"description\": \"The duration the job was queued before execution, in seconds\",\n      \"example\": 42.5\n    },\n    \"ref\": {\n      \"type\": \"string\",\n      \"description\": \"The reference for the job\",\n      \"example\": \"main\"\n    },\n    \"artifacts\": {\n      \"type\": \"array\",\n      \"description\": \"The artifacts produced by the job\"\n    },\n    \"tag\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the job is tagged\",\n      \"example\": true\n    },\n    \"web_url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL for accessing the job in the web\
  \ interface\",\n      \"example\": \"https://gitlab.com/example\"\n    },\n    \"project\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ci_job_token_scope_enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates if the CI/CD job token scope setting is enabled for the project\"\n        }\n      }\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/API_Entities_UserBasic\",\n      \"description\": \"The user that started the job\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-projects-api_entities_job-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_Job
---
