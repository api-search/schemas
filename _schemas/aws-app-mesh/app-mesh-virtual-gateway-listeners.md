---
description: VirtualGatewayListeners schema from AWS App Mesh
layout: schema
name: VirtualGatewayListeners
properties_list: []
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-listeners-schema.json
slug: app-mesh-virtual-gateway-listeners
source_filename: app-mesh-virtual-gateway-listeners-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"connectionPool\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/VirtualGatewayConnectionPool\"\n          },\n          {\n            \"description\": \"The connection pool information for the virtual gateway listener.\"\n          }\n        ]\n      },\n      \"healthCheck\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/VirtualGatewayHealthCheckPolicy\"\n          },\n          {\n            \"description\": \"The health check information for the listener.\"\n          }\n        ]\n      },\n      \"portMapping\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/VirtualGatewayPortMapping\"\n          },\n          {\n            \"description\": \"The port mapping information for the listener.\"\n          }\n        ]\n      },\n      \"tls\": {\n        \"allOf\"\
  : [\n          {\n            \"$ref\": \"#/components/schemas/VirtualGatewayListenerTls\"\n          },\n          {\n            \"description\": \"A reference to an object that represents the Transport Layer Security (TLS) properties for the listener.\"\n          }\n        ]\n      }\n    },\n    \"required\": [\n      \"portMapping\"\n    ],\n    \"description\": \"An object that represents a listener for a virtual gateway.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-listeners-schema.json\",\n  \"title\": \"VirtualGatewayListeners\",\n  \"description\": \"VirtualGatewayListeners schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-listeners-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayListeners
---
