---
description: Represents an API definition managed by the Gravitee APIM platform, including its configuration, lifecycle state, entrypoints, and endpoints.
layout: schema
name: Gravitee API
properties_list:
- description: Unique identifier for the API.
  name: id
  type: string
- description: Name of the API.
  name: name
  type: string
- description: Description of the API.
  name: description
  type: string
- description: Version of the API definition.
  name: version
  type: string
- description: The Gravitee definition version.
  name: definitionVersion
  type: string
- description: 'The type of API: PROXY for synchronous REST/HTTP, MESSAGE for event-driven/async.'
  name: type
  type: string
- description: Current lifecycle state of the API on the gateway.
  name: state
  type: string
- description: Visibility of the API in the developer portal.
  name: visibility
  type: string
- description: Publication lifecycle state of the API.
  name: lifecycleState
  type: string
- description: Sharding tags for gateway routing.
  name: tags
  type: array
- description: Labels for categorization and filtering.
  name: labels
  type: array
- description: API entrypoints defining how consumers connect (v4 APIs).
  name: entrypoints
  type: array
- description: Backend endpoints the gateway proxies to.
  name: endpoints
  type: array
- description: Timestamp of the last deployment to the gateway.
  name: deployedAt
  type: string
- description: Timestamp when the API was created.
  name: createdAt
  type: string
- description: Timestamp when the API was last updated.
  name: updatedAt
  type: string
provider_name: Gravitee
provider_slug: gravitee
schema_file: json-schema/gravitee-api-schema.json
slug: gravitee-api
source_filename: gravitee-api-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://gravitee.io/schemas/gravitee/api.json\",\n  \"title\": \"Gravitee API\",\n  \"description\": \"Represents an API definition managed by the Gravitee APIM platform, including its configuration, lifecycle state, entrypoints, and endpoints.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"version\", \"definitionVersion\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the API definition.\"\n    },\n    \"definitionVersion\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"The Gravitee definition version.\",\n      \"enum\": [\"V2\", \"V4\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of API: PROXY for synchronous REST/HTTP, MESSAGE for event-driven/async.\",\n      \"enum\": [\"PROXY\", \"MESSAGE\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle state of the API on the gateway.\",\n      \"enum\": [\"INITIALIZED\", \"STOPPED\", \"STARTED\", \"CLOSED\"]\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"Visibility of the API in the developer portal.\",\n      \"enum\": [\"PUBLIC\", \"PRIVATE\"]\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"description\": \"Publication lifecycle state of the API.\",\n      \"enum\": [\"CREATED\", \"PUBLISHED\", \"UNPUBLISHED\", \"DEPRECATED\", \"ARCHIVED\"]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Sharding tags for gateway routing.\"\
  ,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels for categorization and filtering.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"entrypoints\": {\n      \"type\": \"array\",\n      \"description\": \"API entrypoints defining how consumers connect (v4 APIs).\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Entrypoint\"\n      }\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"description\": \"Backend endpoints the gateway proxies to.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Endpoint\"\n      }\n    },\n    \"deployedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last deployment to the gateway.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API was created.\"\n    },\n \
  \   \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"Entrypoint\": {\n      \"type\": \"object\",\n      \"description\": \"Defines how consumers connect to the API.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Entrypoint connector type (e.g., http-proxy, websocket, sse).\"\n        },\n        \"configuration\": {\n          \"type\": \"object\",\n          \"description\": \"Entrypoint-specific configuration.\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"Endpoint\": {\n      \"type\": \"object\",\n      \"description\": \"Defines a backend target the gateway proxies requests to.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the endpoint.\"\n        },\n        \"target\": {\n  \
  \        \"type\": \"string\",\n          \"description\": \"Target URL for the backend service.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Endpoint connector type.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gravitee/refs/heads/main/json-schema/gravitee-api-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Gravitee API
---
