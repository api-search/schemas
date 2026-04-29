---
description: An organization on the WSO2 Choreo platform, serving as the top-level grouping for projects, components, APIs, and environments.
layout: schema
name: Choreo Organization
properties_list:
- description: Unique identifier for the organization.
  name: id
  type: string
- description: Name of the organization.
  name: name
  type: string
- description: URL-friendly handle for the organization.
  name: handle
  type: string
- description: Timestamp when the organization was created.
  name: createdAt
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-organization.json
slug: choreo-organization
source_filename: choreo-organization.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-organization.json\",\n  \"title\": \"Choreo Organization\",\n  \"description\": \"An organization on the WSO2 Choreo platform, serving as the top-level grouping for projects, components, APIs, and environments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the organization.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the organization.\"\n    },\n    \"handle\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly handle for the organization.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the organization was created.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"\
  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-organization.json
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
title: Choreo Organization
---
