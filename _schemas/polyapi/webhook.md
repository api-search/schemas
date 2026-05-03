---
description: A webhook endpoint that receives events via HTTP calls, with support for authentication and custom listeners that can be connected to server functions via triggers.
layout: schema
name: PolyAPI Webhook
properties_list:
- description: The unique identifier of the webhook.
  name: id
  type: string
- description: The name of the webhook.
  name: name
  type: string
- description: A description of the webhook.
  name: description
  type: string
- description: The context path for organizing the webhook in the catalog.
  name: context
  type: string
- description: The webhook endpoint URL.
  name: url
  type: string
- description: Authentication configuration for the webhook.
  name: authentication
  type: object
- description: The state of the webhook.
  name: state
  type: string
- description: Timestamp when the webhook was created.
  name: createdAt
  type: string
- description: Timestamp when the webhook was last updated.
  name: updatedAt
  type: string
provider_name: PolyAPI
provider_slug: polyapi
schema_file: json-schema/webhook.json
slug: webhook
source_filename: webhook.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/polyapi/blob/main/json-schema/webhook.json\",\n  \"title\": \"PolyAPI Webhook\",\n  \"description\": \"A webhook endpoint that receives events via HTTP calls, with support for authentication and custom listeners that can be connected to server functions via triggers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the webhook.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the webhook.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the webhook.\"\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"The context path for organizing the webhook in the catalog.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"\
  uri\",\n      \"description\": \"The webhook endpoint URL.\"\n    },\n    \"authentication\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication configuration for the webhook.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\"],\n      \"description\": \"The state of the webhook.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the webhook was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the webhook was last updated.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/json-schema/webhook.json
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
title: PolyAPI Webhook
---
