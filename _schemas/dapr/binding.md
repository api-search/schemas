---
description: Represents a Dapr binding request used to invoke output bindings or receive events from input bindings. Bindings enable integration with external resources such as Kafka, RabbitMQ, Azure Event Hubs, AWS SQS, and GCP Storage.
layout: schema
name: Dapr Binding
properties_list:
- description: The data to send to the output binding.
  name: data
  type: object
- description: Additional metadata for the binding invocation.
  name: metadata
  type: object
- description: The operation to perform on the binding (e.g., create, get, delete, list).
  name: operation
  type: string
provider_name: Dapr
provider_slug: dapr
schema_file: json-schema/binding.json
slug: binding
source_filename: binding.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/dapr/blob/main/json-schema/binding.json\",\n  \"title\": \"Dapr Binding\",\n  \"description\": \"Represents a Dapr binding request used to invoke output bindings or receive events from input bindings. Bindings enable integration with external resources such as Kafka, RabbitMQ, Azure Event Hubs, AWS SQS, and GCP Storage.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"operation\"\n  ],\n  \"properties\": {\n    \"data\": {\n      \"description\": \"The data to send to the output binding.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional metadata for the binding invocation.\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"The operation to perform on the binding (e.g., create, get, delete, list).\"\n\
  \    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/json-schema/binding.json
tags:
- Distributed Systems
- Microservices
- Platform
- Pub/Sub
- State Management
- Workflows
title: Dapr Binding
---
