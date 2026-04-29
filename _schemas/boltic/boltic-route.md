---
description: A route in the Boltic Gateway that defines how incoming API requests are matched and forwarded to backend services.
layout: schema
name: Boltic Gateway Route
properties_list:
- description: Unique identifier for the route
  name: id
  type: string
- description: Human-readable name for the route
  name: name
  type: string
- description: HTTP methods this route responds to
  name: methods
  type: array
- description: URL paths that match this route
  name: paths
  type: array
- description: ID of the backend service to route to
  name: serviceId
  type: string
- description: Whether to strip the matched path prefix before forwarding
  name: stripPath
  type: boolean
- description: Whether to preserve the original Host header
  name: preserveHost
  type: boolean
- description: ''
  name: protocols
  type: array
- description: List of plugin IDs applied to this route
  name: plugins
  type: array
- description: ''
  name: status
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Boltic
provider_slug: boltic
schema_file: json-schema/boltic-route.json
slug: boltic-route
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/json-schema/boltic-route.json\",\n  \"title\": \"Boltic Gateway Route\",\n  \"description\": \"A route in the Boltic Gateway that defines how incoming API requests are matched and forwarded to backend services.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"paths\", \"serviceId\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the route\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the route\"\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"GET\", \"POST\", \"PUT\", \"DELETE\", \"PATCH\", \"OPTIONS\", \"HEAD\"]\n      },\n      \"description\": \"HTTP methods this route responds to\"\n    },\n    \"\
  paths\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"URL paths that match this route\"\n    },\n    \"serviceId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the backend service to route to\"\n    },\n    \"stripPath\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to strip the matched path prefix before forwarding\"\n    },\n    \"preserveHost\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to preserve the original Host header\"\n    },\n    \"protocols\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"http\", \"https\"]\n      }\n    },\n    \"plugins\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of plugin IDs applied to this route\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"\
  inactive\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/json-schema/boltic-route.json
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
title: Boltic Gateway Route
---
