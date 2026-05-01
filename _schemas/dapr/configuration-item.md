---
description: Represents a configuration item retrieved from a Dapr configuration store. Configuration items include a value, version, and optional metadata, and can be subscribed to for real-time change notifications.
layout: schema
name: Dapr ConfigurationItem
properties_list:
- description: The configuration item key.
  name: key
  type: string
- description: The configuration item value.
  name: value
  type: string
- description: The version of the configuration item.
  name: version
  type: string
- description: Additional metadata associated with the configuration item.
  name: metadata
  type: object
provider_name: Dapr
provider_slug: dapr
schema_file: json-schema/configuration-item.json
slug: configuration-item
source_filename: configuration-item.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/dapr/blob/main/json-schema/configuration-item.json\",\n  \"title\": \"Dapr ConfigurationItem\",\n  \"description\": \"Represents a configuration item retrieved from a Dapr configuration store. Configuration items include a value, version, and optional metadata, and can be subscribed to for real-time change notifications.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"value\"\n  ],\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The configuration item key.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The configuration item value.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the configuration item.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\
  \n      },\n      \"description\": \"Additional metadata associated with the configuration item.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/json-schema/configuration-item.json
tags:
- Distributed Systems
- Microservices
- Platform
- Pub/Sub
- State Management
- Workflows
title: Dapr ConfigurationItem
---
