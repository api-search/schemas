---
description: A CircleCI workflow organizes a set of jobs and defines the order, dependencies, and conditions under which they run within a pipeline.
layout: schema
name: CircleCI Workflow
properties_list:
- description: The unique identifier of the pipeline this workflow belongs to
  name: pipeline_id
  type: string
- description: The unique identifier of the workflow
  name: id
  type: string
- description: The name of the workflow as defined in the CircleCI configuration
  name: name
  type: string
- description: The project slug in vcs-slug/org-name/repo-name format
  name: project_slug
  type: string
- description: The current status of the workflow
  name: status
  type: string
- description: The ID of the user who started the workflow
  name: started_by
  type: string
- description: The pipeline number
  name: pipeline_number
  type: integer
- description: When the workflow was created
  name: created_at
  type: string
- description: When the workflow stopped, null if still running
  name: stopped_at
  type:
  - string
  - 'null'
- description: Tag for special workflow types like setup workflows
  name: tag
  type: string
provider_name: CircleCI
provider_slug: circleci
schema_file: json-schema/circleci-workflow-schema.json
slug: circleci-workflow
source_filename: circleci-workflow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://circleci.com/schemas/circleci/workflow.json\",\n  \"title\": \"CircleCI Workflow\",\n  \"description\": \"A CircleCI workflow organizes a set of jobs and defines the order, dependencies, and conditions under which they run within a pipeline.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\", \"pipeline_id\", \"created_at\"],\n  \"properties\": {\n    \"pipeline_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the pipeline this workflow belongs to\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the workflow\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workflow as defined in the CircleCI configuration\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n   \
  \ },\n    \"project_slug\": {\n      \"type\": \"string\",\n      \"description\": \"The project slug in vcs-slug/org-name/repo-name format\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"success\",\n        \"running\",\n        \"not_run\",\n        \"failed\",\n        \"error\",\n        \"failing\",\n        \"on_hold\",\n        \"canceled\",\n        \"unauthorized\"\n      ],\n      \"description\": \"The current status of the workflow\"\n    },\n    \"started_by\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The ID of the user who started the workflow\"\n    },\n    \"pipeline_number\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The pipeline number\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the workflow was created\"\n    },\n    \"stopped_at\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the workflow stopped, null if still running\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"enum\": [\"setup\"],\n      \"description\": \"Tag for special workflow types like setup workflows\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/json-schema/circleci-workflow-schema.json
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
title: CircleCI Workflow
---
