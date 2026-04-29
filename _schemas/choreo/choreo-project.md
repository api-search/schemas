---
description: A project within a Choreo organization, used to group related components, services, and APIs.
layout: schema
name: Choreo Project
properties_list:
- description: Unique identifier for the project.
  name: id
  type: string
- description: Name of the project.
  name: name
  type: string
- description: Description of the project.
  name: description
  type: string
- description: Organization identifier the project belongs to.
  name: orgId
  type: string
- description: Timestamp when the project was created.
  name: createdAt
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-project.json
slug: choreo-project
source_filename: choreo-project.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-project.json\",\n  \"title\": \"Choreo Project\",\n  \"description\": \"A project within a Choreo organization, used to group related components, services, and APIs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the project.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the project.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"Organization identifier the project belongs to.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project\
  \ was created.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"orgId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-project.json
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
title: Choreo Project
---
