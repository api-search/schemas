---
description: A Rollbar deployment record representing a code release. Deploys are used to correlate error spikes with specific releases and track which code version introduced issues.
layout: schema
name: Rollbar Deploy
properties_list:
- description: The deploy ID assigned by Rollbar.
  name: id
  type: integer
- description: The project ID this deploy belongs to.
  name: project_id
  type: integer
- description: The environment deployed to (e.g., production, staging, development).
  name: environment
  type: string
- description: The revision identifier, typically a Git commit SHA or version string.
  name: revision
  type: string
- description: The local system username of the person who performed the deploy.
  name: local_username
  type: string
- description: The Rollbar username of the person who performed the deploy.
  name: rollbar_username
  type: string
- description: An optional comment describing the deployment or changes included.
  name: comment
  type: string
- description: The status of the deployment lifecycle.
  name: status
  type: string
- description: Unix timestamp when the deploy started.
  name: start_time
  type: integer
- description: Unix timestamp when the deploy finished.
  name: finish_time
  type: integer
- description: The Rollbar user ID who initiated the deploy.
  name: user_id
  type: integer
provider_name: Rollbar
provider_slug: rollbar
schema_file: json-schema/rollbar-deploy-schema.json
slug: rollbar-deploy
source_filename: rollbar-deploy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://rollbar.com/schemas/rollbar/deploy.json\",\n  \"title\": \"Rollbar Deploy\",\n  \"description\": \"A Rollbar deployment record representing a code release. Deploys are used to correlate error spikes with specific releases and track which code version introduced issues.\",\n  \"type\": \"object\",\n  \"required\": [\"environment\", \"revision\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The deploy ID assigned by Rollbar.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The project ID this deploy belongs to.\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"description\": \"The environment deployed to (e.g., production, staging, development).\",\n      \"maxLength\": 255\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"description\": \"The revision identifier,\
  \ typically a Git commit SHA or version string.\",\n      \"maxLength\": 40\n    },\n    \"local_username\": {\n      \"type\": \"string\",\n      \"description\": \"The local system username of the person who performed the deploy.\"\n    },\n    \"rollbar_username\": {\n      \"type\": \"string\",\n      \"description\": \"The Rollbar username of the person who performed the deploy.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"An optional comment describing the deployment or changes included.\",\n      \"maxLength\": 64000\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the deployment lifecycle.\",\n      \"enum\": [\"started\", \"succeeded\", \"failed\", \"timed_out\"]\n    },\n    \"start_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the deploy started.\"\n    },\n    \"finish_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp\
  \ when the deploy finished.\"\n    },\n    \"user_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The Rollbar user ID who initiated the deploy.\"\n    }\n  },\n  \"$defs\": {\n    \"DeployStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle status of a deployment.\",\n      \"enum\": [\"started\", \"succeeded\", \"failed\", \"timed_out\"]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/json-schema/rollbar-deploy-schema.json
tags:
- Error Tracking
- Monitoring
- Debugging
- DevOps
- Application Performance
title: Rollbar Deploy
---
