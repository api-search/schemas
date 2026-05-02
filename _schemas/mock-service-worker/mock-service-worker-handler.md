---
description: Schema describing a Mock Service Worker (MSW) request handler definition. Captures the protocol, matching pattern, and mocked response so handler definitions can be portable across MSW environments.
layout: schema
name: Mock Service Worker Handler
properties_list: []
provider_name: Mock Service Worker
provider_slug: mock-service-worker
schema_file: json-schema/mock-service-worker-handler-schema.json
slug: mock-service-worker-handler
source_filename: mock-service-worker-handler-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/mock-service-worker/main/json-schema/mock-service-worker-handler-schema.json\",\n  \"title\": \"Mock Service Worker Handler\",\n  \"description\": \"Schema describing a Mock Service Worker (MSW) request handler definition. Captures the protocol, matching pattern, and mocked response so handler definitions can be portable across MSW environments.\",\n  \"type\": \"object\",\n  \"required\": [\"protocol\"],\n  \"oneOf\": [\n    {\n      \"title\": \"REST handler\",\n      \"properties\": {\n        \"protocol\": { \"const\": \"http\" },\n        \"method\": {\n          \"type\": \"string\",\n          \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"HEAD\", \"OPTIONS\", \"ALL\"]\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"URL pattern, supports path parameters via :param syntax.\"\n\
  \        },\n        \"response\": { \"$ref\": \"#/$defs/response\" }\n      },\n      \"required\": [\"protocol\", \"method\", \"path\"]\n    },\n    {\n      \"title\": \"GraphQL handler\",\n      \"properties\": {\n        \"protocol\": { \"const\": \"graphql\" },\n        \"operationKind\": { \"type\": \"string\", \"enum\": [\"query\", \"mutation\", \"subscription\", \"operation\"] },\n        \"operationName\": { \"type\": \"string\" },\n        \"endpoint\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"response\": { \"$ref\": \"#/$defs/response\" }\n      },\n      \"required\": [\"protocol\", \"operationKind\"]\n    },\n    {\n      \"title\": \"WebSocket handler\",\n      \"properties\": {\n        \"protocol\": { \"const\": \"ws\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n      },\n      \"required\": [\"protocol\", \"url\"]\n    },\n    {\n      \"title\": \"Server-Sent Events handler\",\n      \"properties\": {\n        \"protocol\": {\
  \ \"const\": \"sse\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n      },\n      \"required\": [\"protocol\", \"url\"]\n    }\n  ],\n  \"$defs\": {\n    \"response\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"status\": { \"type\": \"integer\", \"minimum\": 100, \"maximum\": 599 },\n        \"headers\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"body\": {},\n        \"delayMs\": { \"type\": \"integer\", \"minimum\": 0 }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mock-service-worker/refs/heads/main/json-schema/mock-service-worker-handler-schema.json
tags:
- API Mocking
- GraphQL
- HTTP
- Mock Server
- Mocking
- Service Worker
- Testing
- WebSocket
title: Mock Service Worker Handler
---
