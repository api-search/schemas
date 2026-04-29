---
description: An object that represents a type of connection pool.
layout: schema
name: VirtualGatewayHttp2ConnectionPool
properties_list:
- description: ''
  name: maxRequests
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-http2-connection-pool-schema.json
slug: app-mesh-virtual-gateway-http2-connection-pool
source_filename: app-mesh-virtual-gateway-http2-connection-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxRequests\"\n        },\n        {\n          \"description\": \"Maximum number of inflight requests Envoy can concurrently support across hosts in upstream cluster.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"maxRequests\"\n  ],\n  \"description\": \"An object that represents a type of connection pool.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-http2-connection-pool-schema.json\",\n  \"title\": \"VirtualGatewayHttp2ConnectionPool\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-http2-connection-pool-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayHttp2ConnectionPool
---
