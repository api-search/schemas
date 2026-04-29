---
description: A deployment environment within a Choreo organization, such as Development, Staging, or Production.
layout: schema
name: Choreo Environment
properties_list:
- description: Unique identifier for the environment.
  name: id
  type: string
- description: Name of the environment.
  name: name
  type: string
- description: Type of the environment.
  name: type
  type: string
- description: Whether this is the default environment.
  name: isDefault
  type: boolean
- description: Organization identifier this environment belongs to.
  name: orgId
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-environment.json
slug: choreo-environment
source_filename: choreo-environment.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-environment.json\",\n  \"title\": \"Choreo Environment\",\n  \"description\": \"A deployment environment within a Choreo organization, such as Development, Staging, or Production.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the environment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the environment.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"Development\", \"Staging\", \"Production\"],\n      \"description\": \"Type of the environment.\"\n    },\n    \"isDefault\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the default environment.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Organization identifier this environment belongs to.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-environment.json
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
title: Choreo Environment
---
