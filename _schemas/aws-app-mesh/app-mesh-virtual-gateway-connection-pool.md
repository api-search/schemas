---
description: <p>An object that represents the type of virtual gateway connection pool.</p> <p>Only one protocol is used at a time and should be the same protocol as the one chosen under port mapping.</p> <p>If not present the default value for <code>maxPendingRequests</code> is <code>2147483647</code>.</p>
layout: schema
name: VirtualGatewayConnectionPool
properties_list:
- description: ''
  name: grpc
  type: object
- description: ''
  name: http
  type: object
- description: ''
  name: http2
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-connection-pool-schema.json
slug: app-mesh-virtual-gateway-connection-pool
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"grpc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayGrpcConnectionPool\"\n        },\n        {\n          \"description\": \"An object that represents a type of connection pool. \"\n        }\n      ]\n    },\n    \"http\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayHttpConnectionPool\"\n        },\n        {\n          \"description\": \"An object that represents a type of connection pool.\"\n        }\n      ]\n    },\n    \"http2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayHttp2ConnectionPool\"\n        },\n        {\n          \"description\": \"An object that represents a type of connection pool.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>An object that represents the type of virtual gateway connection pool.</p> <p>Only one protocol is used at a time and\
  \ should be the same protocol as the one chosen under port mapping.</p> <p>If not present the default value for <code>maxPendingRequests</code> is <code>2147483647</code>.</p>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-connection-pool-schema.json\",\n  \"title\": \"VirtualGatewayConnectionPool\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-connection-pool-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayConnectionPool
---
