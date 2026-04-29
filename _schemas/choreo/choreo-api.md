---
description: A managed API published through the Choreo API gateway, supporting REST, GraphQL, gRPC, and WebSocket types with lifecycle management.
layout: schema
name: Choreo API
properties_list:
- description: Unique identifier for the API.
  name: id
  type: string
- description: Name of the API.
  name: name
  type: string
- description: Version of the API.
  name: version
  type: string
- description: Context path of the API.
  name: context
  type: string
- description: Type of the API.
  name: type
  type: string
- description: Lifecycle status of the API.
  name: status
  type: string
- description: Visibility scope of the API.
  name: visibility
  type: string
- description: Component identifier the API is associated with.
  name: componentId
  type: string
- description: Timestamp when the API was created.
  name: createdAt
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-api.json
slug: choreo-api
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-api.json\",\n  \"title\": \"Choreo API\",\n  \"description\": \"A managed API published through the Choreo API gateway, supporting REST, GraphQL, gRPC, and WebSocket types with lifecycle management.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the API.\"\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"Context path of the API.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"REST\", \"GraphQL\", \"gRPC\", \"WebSocket\"],\n      \"description\": \"Type\
  \ of the API.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Created\", \"Published\", \"Deprecated\", \"Retired\"],\n      \"description\": \"Lifecycle status of the API.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"Public\", \"Organization\", \"Project\"],\n      \"description\": \"Visibility scope of the API.\"\n    },\n    \"componentId\": {\n      \"type\": \"string\",\n      \"description\": \"Component identifier the API is associated with.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API was created.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-api.json
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
title: Choreo API
---
