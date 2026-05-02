---
description: An Integration represents a Camel-based integration project containing routes, configurations, and an optional Git repository connection for building and deploying data flows on Kubernetes.
layout: schema
name: Jetic Integration
properties_list:
- description: Unique identifier for the integration.
  name: id
  type: string
- description: Name of the integration project.
  name: name
  type: string
- description: Description of the integration.
  name: description
  type: string
- description: Current status of the integration.
  name: status
  type: string
- description: Camel routes defined within this integration.
  name: routes
  type: array
- description: Connected Git repository URL.
  name: gitRepository
  type: string
- description: Timestamp when the integration was created.
  name: createdAt
  type: string
- description: Timestamp when the integration was last updated.
  name: updatedAt
  type: string
provider_name: Jetic
provider_slug: jetic
schema_file: json-schema/integration.json
slug: integration
source_filename: integration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/jetic/blob/main/json-schema/integration.json\",\n  \"title\": \"Jetic Integration\",\n  \"description\": \"An Integration represents a Camel-based integration project containing routes, configurations, and an optional Git repository connection for building and deploying data flows on Kubernetes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the integration.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the integration project.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the integration.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"draft\",\n        \"deployed\",\n        \"stopped\",\n        \"error\"\n      ],\n      \"\
  description\": \"Current status of the integration.\"\n    },\n    \"routes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"route.json\"\n      },\n      \"description\": \"Camel routes defined within this integration.\"\n    },\n    \"gitRepository\": {\n      \"type\": \"string\",\n      \"description\": \"Connected Git repository URL.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the integration was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the integration was last updated.\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/json-schema/integration.json
tags:
- Apache Camel
- Integrations
- iPaaS
- Pro-Code API Composition
title: Jetic Integration
---
