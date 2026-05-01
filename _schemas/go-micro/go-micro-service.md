---
description: JSON Schema representing a Go Micro service definition, including service metadata, endpoint registration, and node information as exposed via the registry.
layout: schema
name: Go Micro Service Definition
properties_list:
- description: Unique service name used for discovery and routing.
  name: name
  type: string
- description: Service version string.
  name: version
  type: string
- description: Custom key-value metadata for the service.
  name: metadata
  type: object
- description: List of RPC endpoints exposed by the service.
  name: endpoints
  type: array
- description: Registered nodes running this service.
  name: nodes
  type: array
provider_name: Go Micro
provider_slug: go-micro
schema_file: json-schema/go-micro-service.json
slug: go-micro-service
source_filename: go-micro-service.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/go-micro/json-schema/go-micro-service.json\",\n  \"title\": \"Go Micro Service Definition\",\n  \"description\": \"JSON Schema representing a Go Micro service definition, including service metadata, endpoint registration, and node information as exposed via the registry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique service name used for discovery and routing.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Service version string.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom key-value metadata for the service.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"description\": \"List of RPC endpoints exposed\
  \ by the service.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Fully qualified endpoint name (e.g., Greeter.Hello).\"\n          },\n          \"request\": {\n            \"type\": \"object\",\n            \"description\": \"Request type information.\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Request message type name.\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Request type (e.g., protobuf message name).\"\n              }\n            },\n            \"additionalProperties\": true\n          },\n          \"response\": {\n            \"type\": \"object\",\n            \"description\": \"Response type information.\",\n            \"properties\": {\n              \"name\": {\n                \"\
  type\": \"string\",\n                \"description\": \"Response message type name.\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Response type (e.g., protobuf message name).\"\n              }\n            },\n            \"additionalProperties\": true\n          },\n          \"metadata\": {\n            \"type\": \"object\",\n            \"description\": \"Endpoint metadata (e.g., stream, subscriber info).\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"required\": [\"name\"],\n        \"additionalProperties\": true\n      }\n    },\n    \"nodes\": {\n      \"type\": \"array\",\n      \"description\": \"Registered nodes running this service.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique node identifier.\"\
  \n          },\n          \"address\": {\n            \"type\": \"string\",\n            \"description\": \"Node address (host:port).\"\n          },\n          \"metadata\": {\n            \"type\": \"object\",\n            \"description\": \"Node-level metadata (e.g., transport, broker, protocol).\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"required\": [\"id\", \"address\"],\n        \"additionalProperties\": true\n      }\n    }\n  },\n  \"required\": [\"name\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/go-micro/refs/heads/main/json-schema/go-micro-service.json
tags:
- Distributed Systems
- Frameworks
- Go
- Golang
- Microservices
- RPC
- Service Discovery
title: Go Micro Service Definition
---
