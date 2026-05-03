---
description: Represents a data source connection configuration in Orbital, defining how Orbital connects to external APIs, databases, message queues, or serverless functions.
layout: schema
name: Orbital Connection
properties_list:
- description: Unique identifier for the connection.
  name: connectionId
  type: string
- description: Display name of the connection.
  name: name
  type: string
- description: Type of the data source connection.
  name: connectionType
  type: string
- description: URL or connection string for the data source.
  name: connectionUrl
  type: string
- description: Current status of the connection.
  name: status
  type: string
- description: Authentication configuration for the connection.
  name: authentication
  type: object
provider_name: Orbital
provider_slug: orbital
schema_file: json-schema/connection.json
slug: connection
source_filename: connection.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/connection.json\",\n  \"title\": \"Orbital Connection\",\n  \"description\": \"Represents a data source connection configuration in Orbital, defining how Orbital connects to external APIs, databases, message queues, or serverless functions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the connection.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the connection.\"\n    },\n    \"connectionType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the data source connection.\",\n      \"enum\": [\"API\", \"DATABASE\", \"MESSAGE_QUEUE\", \"SERVERLESS_FUNCTION\"]\n    },\n    \"connectionUrl\": {\n      \"type\": \"string\",\n      \"format\": \"\
  uri\",\n      \"description\": \"URL or connection string for the data source.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the connection.\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\", \"ERROR\"]\n    },\n    \"authentication\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication configuration for the connection.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Authentication method.\",\n          \"enum\": [\"NONE\", \"BASIC\", \"BEARER_TOKEN\", \"OAUTH2\", \"API_KEY\"]\n        },\n        \"credentials\": {\n          \"type\": \"object\",\n          \"description\": \"Authentication credentials (format depends on auth type).\",\n          \"additionalProperties\": true\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"connectionType\", \"connectionUrl\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/connection.json
tags:
- Data
- Gateways
title: Orbital Connection
---
