---
description: Represents a state key/value pair used in Dapr state management operations, including optional concurrency control via ETags and metadata.
layout: schema
name: Dapr StateItem
properties_list:
- description: The state key identifier.
  name: key
  type: string
- description: The state value. Can be any JSON-serializable value.
  name: value
  type: object
- description: ETag for optimistic concurrency control.
  name: etag
  type: string
- description: Additional key/value metadata for the state operation.
  name: metadata
  type: object
- description: Options for concurrency and consistency behavior.
  name: options
  type: object
provider_name: Dapr
provider_slug: dapr
schema_file: json-schema/state-item.json
slug: state-item
source_filename: state-item.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/dapr/blob/main/json-schema/state-item.json\",\n  \"title\": \"Dapr StateItem\",\n  \"description\": \"Represents a state key/value pair used in Dapr state management operations, including optional concurrency control via ETags and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"key\",\n    \"value\"\n  ],\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The state key identifier.\"\n    },\n    \"value\": {\n      \"description\": \"The state value. Can be any JSON-serializable value.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for optimistic concurrency control.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional key/value metadata for the state\
  \ operation.\"\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"description\": \"Options for concurrency and consistency behavior.\",\n      \"properties\": {\n        \"concurrency\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"first-write\",\n            \"last-write\"\n          ],\n          \"description\": \"Concurrency mode for the state operation.\"\n        },\n        \"consistency\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"eventual\",\n            \"strong\"\n          ],\n          \"description\": \"Consistency level for the state operation.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/json-schema/state-item.json
tags:
- Distributed Systems
- Microservices
- Platform
- Pub/Sub
- State Management
- Workflows
title: Dapr StateItem
---
