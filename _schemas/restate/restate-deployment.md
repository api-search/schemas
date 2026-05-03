---
description: Represents a Restate service deployment registration — a URI endpoint that hosts one or more durable services.
layout: schema
name: Deployment
properties_list:
- description: Unique identifier for the deployment.
  name: id
  type: string
- description: The URI of the service deployment endpoint.
  name: uri
  type: string
- description: The HTTP protocol type used for communication.
  name: protocol_type
  type: string
- description: The HTTP version used (e.g., HTTP_2, HTTP_11).
  name: http_version
  type: string
- description: Additional HTTP headers to include when calling the deployment.
  name: additional_headers
  type: object
- description: ISO 8601 timestamp when the deployment was registered.
  name: created_at
  type: string
- description: List of services hosted by this deployment.
  name: services
  type: array
provider_name: Restate
provider_slug: restate
schema_file: json-schema/restate-deployment-schema.json
slug: restate-deployment
source_filename: restate-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/json-schema/restate-deployment-schema.json\",\n  \"title\": \"Deployment\",\n  \"description\": \"Represents a Restate service deployment registration — a URI endpoint that hosts one or more durable services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the deployment.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URI of the service deployment endpoint.\"\n    },\n    \"protocol_type\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP protocol type used for communication.\",\n      \"enum\": [\"RequestResponse\", \"BidiStream\"]\n    },\n    \"http_version\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP version used (e.g., HTTP_2,\
  \ HTTP_11).\"\n    },\n    \"additional_headers\": {\n      \"type\": \"object\",\n      \"description\": \"Additional HTTP headers to include when calling the deployment.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the deployment was registered.\"\n    },\n    \"services\": {\n      \"type\": \"array\",\n      \"description\": \"List of services hosted by this deployment.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ServiceMetadata\"\n      }\n    }\n  },\n  \"required\": [\"id\", \"uri\"],\n  \"$defs\": {\n    \"ServiceMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata for a Restate service.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The service name.\"\n        },\n        \"ty\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The service type.\",\n          \"enum\": [\"Service\", \"VirtualObject\", \"Workflow\"]\n        },\n        \"deployment_id\": {\n          \"type\": \"string\",\n          \"description\": \"The deployment that hosts this service.\"\n        },\n        \"revision\": {\n          \"type\": \"integer\",\n          \"description\": \"The service revision number.\"\n        },\n        \"public\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the service is publicly accessible.\"\n        },\n        \"idempotency_retention\": {\n          \"type\": \"string\",\n          \"description\": \"Duration for retaining idempotency keys.\"\n        },\n        \"workflow_completion_retention\": {\n          \"type\": \"string\",\n          \"description\": \"Duration for retaining workflow completion state.\"\n        },\n        \"handlers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/HandlerMetadata\"\
  \n          }\n        }\n      },\n      \"required\": [\"name\", \"ty\"]\n    },\n    \"HandlerMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata for a durable handler within a service.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The handler name.\"\n        },\n        \"ty\": {\n          \"type\": \"string\",\n          \"description\": \"The handler type.\",\n          \"enum\": [\"Exclusive\", \"Shared\", \"Workflow\"]\n        },\n        \"input\": {\n          \"type\": \"object\",\n          \"description\": \"Input schema for the handler.\",\n          \"properties\": {\n            \"required\": {\"type\": \"boolean\"},\n            \"contentType\": {\"type\": \"string\"},\n            \"jsonSchema\": {\"type\": \"object\"}\n          }\n        },\n        \"output\": {\n          \"type\": \"object\",\n          \"description\": \"Output schema for the handler.\",\n          \"\
  properties\": {\n            \"contentType\": {\"type\": \"string\"},\n            \"setContentTypeIfEmpty\": {\"type\": \"boolean\"},\n            \"jsonSchema\": {\"type\": \"object\"}\n          }\n        }\n      },\n      \"required\": [\"name\", \"ty\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/json-schema/restate-deployment-schema.json
tags:
- Durable Execution
- Workflows
- Microservices
- Orchestration
- Distributed Systems
title: Deployment
---
