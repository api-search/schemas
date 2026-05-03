---
description: Represents a service connected to Orbital, such as a REST API, gRPC service, database, or message queue.
layout: schema
name: Orbital Service
properties_list:
- description: Name of the service.
  name: name
  type: string
- description: Base URL of the service.
  name: url
  type: string
- description: Protocol type of the service.
  name: protocol
  type: string
- description: Number of operations exposed by this service.
  name: operationCount
  type: integer
- description: Current connection status of the service.
  name: status
  type: string
- description: Operations exposed by this service.
  name: operations
  type: array
- description: Types exposed by this service.
  name: types
  type: array
provider_name: Orbital
provider_slug: orbital
schema_file: json-schema/service.json
slug: service
source_filename: service.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/service.json\",\n  \"title\": \"Orbital Service\",\n  \"description\": \"Represents a service connected to Orbital, such as a REST API, gRPC service, database, or message queue.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the service.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Base URL of the service.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"Protocol type of the service.\",\n      \"enum\": [\"REST\", \"gRPC\", \"SOAP\", \"Kafka\", \"Database\"]\n    },\n    \"operationCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of operations exposed by this service.\"\n    },\n    \"status\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Current connection status of the service.\",\n      \"enum\": [\"CONNECTED\", \"DISCONNECTED\", \"ERROR\"]\n    },\n    \"operations\": {\n      \"type\": \"array\",\n      \"description\": \"Operations exposed by this service.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Operation name.\"\n          },\n          \"returnType\": {\n            \"type\": \"string\",\n            \"description\": \"Qualified type name of the return type.\"\n          },\n          \"parameters\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                },\n                \"type\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n \
  \         }\n        }\n      }\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"Types exposed by this service.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"name\", \"protocol\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/service.json
tags:
- Data
- Gateways
title: Orbital Service
---
