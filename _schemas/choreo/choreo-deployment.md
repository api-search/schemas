---
description: A deployment of a built component artifact to a target environment on the Choreo platform.
layout: schema
name: Choreo Deployment
properties_list:
- description: Unique identifier for the deployment.
  name: id
  type: string
- description: Component identifier being deployed.
  name: componentId
  type: string
- description: Build identifier being deployed.
  name: buildId
  type: string
- description: Target environment identifier.
  name: environmentId
  type: string
- description: Current status of the deployment.
  name: status
  type: string
- description: Timestamp when the deployment was created.
  name: createdAt
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-deployment.json
slug: choreo-deployment
source_filename: choreo-deployment.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-deployment.json\",\n  \"title\": \"Choreo Deployment\",\n  \"description\": \"A deployment of a built component artifact to a target environment on the Choreo platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the deployment.\"\n    },\n    \"componentId\": {\n      \"type\": \"string\",\n      \"description\": \"Component identifier being deployed.\"\n    },\n    \"buildId\": {\n      \"type\": \"string\",\n      \"description\": \"Build identifier being deployed.\"\n    },\n    \"environmentId\": {\n      \"type\": \"string\",\n      \"description\": \"Target environment identifier.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Pending\", \"Active\", \"Failed\", \"Inactive\"\
  ],\n      \"description\": \"Current status of the deployment.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment was created.\"\n    }\n  },\n  \"required\": [\"id\", \"buildId\", \"environmentId\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-deployment.json
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
title: Choreo Deployment
---
