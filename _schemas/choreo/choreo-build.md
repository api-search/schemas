---
description: A build triggered for a Choreo component, representing the CI process of compiling and packaging component source code.
layout: schema
name: Choreo Build
properties_list:
- description: Unique identifier for the build.
  name: id
  type: string
- description: Component identifier this build belongs to.
  name: componentId
  type: string
- description: Current status of the build.
  name: status
  type: string
- description: Git commit hash the build was triggered from.
  name: commitHash
  type: string
- description: Git branch the build was triggered from.
  name: branch
  type: string
- description: Timestamp when the build was created.
  name: createdAt
  type: string
- description: Timestamp when the build completed.
  name: completedAt
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-build.json
slug: choreo-build
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-build.json\",\n  \"title\": \"Choreo Build\",\n  \"description\": \"A build triggered for a Choreo component, representing the CI process of compiling and packaging component source code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the build.\"\n    },\n    \"componentId\": {\n      \"type\": \"string\",\n      \"description\": \"Component identifier this build belongs to.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Pending\", \"InProgress\", \"Success\", \"Failed\", \"Cancelled\"],\n      \"description\": \"Current status of the build.\"\n    },\n    \"commitHash\": {\n      \"type\": \"string\",\n      \"description\": \"Git commit hash the build was triggered from.\"\n   \
  \ },\n    \"branch\": {\n      \"type\": \"string\",\n      \"description\": \"Git branch the build was triggered from.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the build was created.\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the build completed.\"\n    }\n  },\n  \"required\": [\"id\", \"componentId\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-build.json
tags:
- AI Apps
- API Management
- CI/CD
- Cloud Native
- DevOps
- Developer Portal
- FinOps
- IDE
- Internal Developer Platform
- Kubernetes
- Lifecycle
- Observability
- Orchestration
- Platform Engineering
- Pro-Code API Composition
- Unified
- WSO2
- Workflows
title: Choreo Build
---
