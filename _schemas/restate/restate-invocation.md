---
description: Represents a Restate durable invocation — an in-flight or completed call to a service handler with exactly-once execution semantics.
layout: schema
name: Invocation
properties_list:
- description: Unique identifier for the invocation.
  name: id
  type: string
- description: The fully qualified target in format ServiceName/handlerName or ServiceName/key/handlerName.
  name: target
  type: string
- description: The name of the target service.
  name: target_service_name
  type: string
- description: The name of the target handler.
  name: target_handler_name
  type: string
- description: The virtual object key (null for plain services).
  name: target_service_key
  type:
  - string
  - 'null'
- description: Current execution status of the invocation.
  name: status
  type: string
- description: ISO 8601 timestamp when the invocation was created.
  name: created_at
  type: string
- description: ISO 8601 timestamp when the invocation status last changed.
  name: modified_at
  type: string
- description: Distributed trace identifier for observability.
  name: trace_id
  type: string
- description: The deployment that is handling this invocation.
  name: deployment_id
  type: string
- description: Number of times this invocation has been retried.
  name: retry_count
  type: integer
- description: Description of the last failure that caused a retry.
  name: last_failure
  type:
  - string
  - 'null'
- description: ISO 8601 timestamp for when the next retry will occur.
  name: next_retry_at
  type:
  - string
  - 'null'
provider_name: Restate
provider_slug: restate
schema_file: json-schema/restate-invocation-schema.json
slug: restate-invocation
source_filename: restate-invocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/json-schema/restate-invocation-schema.json\",\n  \"title\": \"Invocation\",\n  \"description\": \"Represents a Restate durable invocation — an in-flight or completed call to a service handler with exactly-once execution semantics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the invocation.\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified target in format ServiceName/handlerName or ServiceName/key/handlerName.\"\n    },\n    \"target_service_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the target service.\"\n    },\n    \"target_handler_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the target handler.\"\n    },\n\
  \    \"target_service_key\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The virtual object key (null for plain services).\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current execution status of the invocation.\",\n      \"enum\": [\"pending\", \"ready\", \"running\", \"backing-off\", \"suspended\", \"completed\"]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the invocation was created.\"\n    },\n    \"modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the invocation status last changed.\"\n    },\n    \"trace_id\": {\n      \"type\": \"string\",\n      \"description\": \"Distributed trace identifier for observability.\"\n    },\n    \"deployment_id\": {\n      \"type\": \"string\",\n      \"description\": \"The deployment that is handling this invocation.\"\
  \n    },\n    \"retry_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of times this invocation has been retried.\"\n    },\n    \"last_failure\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Description of the last failure that caused a retry.\"\n    },\n    \"next_retry_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp for when the next retry will occur.\"\n    }\n  },\n  \"required\": [\"id\", \"target\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/json-schema/restate-invocation-schema.json
tags:
- Durable Execution
- Workflows
- Microservices
- Orchestration
- Distributed Systems
title: Invocation
---
