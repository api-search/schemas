---
description: JSON Schema for Nameko microservices framework configuration (config.yml).
layout: schema
name: Nameko Service Configuration
properties_list:
- description: AMQP broker connection URI.
  name: AMQP_URI
  type: string
- description: Address for HTTP entrypoints to listen on.
  name: WEB_SERVER_ADDRESS
  type: string
- description: Name of the RPC exchange.
  name: rpc_exchange
  type: string
- description: Maximum number of concurrent workers per service.
  name: max_workers
  type: integer
- description: Number of parent calls tracked for call ID stacks.
  name: parent_calls_tracked
  type: integer
- description: Default serializer for RPC messages.
  name: serializer
  type: string
- description: Accepted content types for deserialization.
  name: ACCEPT_CONTENT
  type: array
- description: AMQP heartbeat interval in seconds.
  name: HEARTBEAT
  type: integer
- description: AMQP consumer prefetch count.
  name: PREFETCH_COUNT
  type: integer
- description: AMQP login method.
  name: LOGIN_METHOD
  type: string
- description: Python logging dictConfig configuration.
  name: LOGGING
  type: object
provider_name: Nameko
provider_slug: nameko
schema_file: json-schema/nameko-configuration.json
slug: nameko-configuration
source_filename: nameko-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nameko/json-schema/nameko-configuration.json\",\n  \"title\": \"Nameko Service Configuration\",\n  \"description\": \"JSON Schema for Nameko microservices framework configuration (config.yml).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AMQP_URI\": {\n      \"type\": \"string\",\n      \"default\": \"pyamqp://guest:guest@localhost\",\n      \"description\": \"AMQP broker connection URI.\"\n    },\n    \"WEB_SERVER_ADDRESS\": {\n      \"type\": \"string\",\n      \"default\": \"0.0.0.0:8000\",\n      \"description\": \"Address for HTTP entrypoints to listen on.\"\n    },\n    \"rpc_exchange\": {\n      \"type\": \"string\",\n      \"default\": \"nameko-rpc\",\n      \"description\": \"Name of the RPC exchange.\"\n    },\n    \"max_workers\": {\n      \"type\": \"integer\",\n      \"default\": 10,\n      \"description\": \"Maximum number of concurrent\
  \ workers per service.\"\n    },\n    \"parent_calls_tracked\": {\n      \"type\": \"integer\",\n      \"default\": 10,\n      \"description\": \"Number of parent calls tracked for call ID stacks.\"\n    },\n    \"serializer\": {\n      \"type\": \"string\",\n      \"default\": \"json\",\n      \"description\": \"Default serializer for RPC messages.\"\n    },\n    \"ACCEPT_CONTENT\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"default\": [\"json\"],\n      \"description\": \"Accepted content types for deserialization.\"\n    },\n    \"HEARTBEAT\": {\n      \"type\": \"integer\",\n      \"default\": 60,\n      \"description\": \"AMQP heartbeat interval in seconds.\"\n    },\n    \"PREFETCH_COUNT\": {\n      \"type\": \"integer\",\n      \"default\": 10,\n      \"description\": \"AMQP consumer prefetch count.\"\n    },\n    \"LOGIN_METHOD\": {\n      \"type\": \"string\",\n      \"description\": \"AMQP login method.\"\n    },\n    \"LOGGING\": {\n \
  \     \"type\": \"object\",\n      \"properties\": {\n        \"version\": { \"type\": \"integer\", \"default\": 1 },\n        \"handlers\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"class\": { \"type\": \"string\" },\n              \"level\": { \"type\": \"string\" },\n              \"formatter\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"root\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"level\": { \"type\": \"string\" },\n            \"handlers\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" }\n            }\n          }\n        }\n      },\n      \"description\": \"Python logging dictConfig configuration.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nameko/refs/heads/main/json-schema/nameko-configuration.json
tags:
- AMQP
- Dependency Injection
- Frameworks
- Microservices
- Python
- RPC
- Testing
title: Nameko Service Configuration
---
