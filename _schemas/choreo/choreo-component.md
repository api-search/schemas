---
description: A deployable component within a Choreo project. Components represent services, API proxies, web applications, scheduled jobs, manual triggers, event handlers, or webhooks.
layout: schema
name: Choreo Component
properties_list:
- description: Unique identifier for the component.
  name: id
  type: string
- description: Name of the component.
  name: name
  type: string
- description: Type of the component.
  name: type
  type: string
- description: Description of the component.
  name: description
  type: string
- description: Git repository URL for the component source code.
  name: repoUrl
  type: string
- description: Git branch used for builds.
  name: branch
  type: string
- description: Buildpack used for the component.
  name: buildpackId
  type: string
- description: Project identifier the component belongs to.
  name: projectId
  type: string
- description: Organization identifier.
  name: orgId
  type: string
- description: Current status of the component.
  name: status
  type: string
- description: Timestamp when the component was created.
  name: createdAt
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-component.json
slug: choreo-component
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-component.json\",\n  \"title\": \"Choreo Component\",\n  \"description\": \"A deployable component within a Choreo project. Components represent services, API proxies, web applications, scheduled jobs, manual triggers, event handlers, or webhooks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the component.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the component.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Service\",\n        \"REST API Proxy\",\n        \"GraphQL API Proxy\",\n        \"Web Application\",\n        \"Scheduled Job\",\n        \"Manual Trigger\",\n        \"Event Handler\",\n        \"Webhook\"\n      ],\n\
  \      \"description\": \"Type of the component.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the component.\"\n    },\n    \"repoUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Git repository URL for the component source code.\"\n    },\n    \"branch\": {\n      \"type\": \"string\",\n      \"description\": \"Git branch used for builds.\"\n    },\n    \"buildpackId\": {\n      \"type\": \"string\",\n      \"description\": \"Buildpack used for the component.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Project identifier the component belongs to.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"Organization identifier.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Inactive\"],\n      \"description\": \"Current status of the component.\"\n    },\n    \"createdAt\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the component was created.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-component.json
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
title: Choreo Component
---
