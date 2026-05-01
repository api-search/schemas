---
description: An object that represents a type of connection pool.
layout: schema
name: VirtualNodeHttpConnectionPool
properties_list:
- description: ''
  name: maxConnections
  type: object
- description: ''
  name: maxPendingRequests
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-node-http-connection-pool-schema.json
slug: app-mesh-virtual-node-http-connection-pool
source_filename: app-mesh-virtual-node-http-connection-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxConnections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxConnections\"\n        },\n        {\n          \"description\": \"Maximum number of outbound TCP connections Envoy can establish concurrently with all hosts in upstream cluster.\"\n        }\n      ]\n    },\n    \"maxPendingRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxPendingRequests\"\n        },\n        {\n          \"description\": \"Number of overflowing requests after <code>max_connections</code> Envoy will queue to upstream cluster.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"maxConnections\"\n  ],\n  \"description\": \"An object that represents a type of connection pool.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-node-http-connection-pool-schema.json\"\
  ,\n  \"title\": \"VirtualNodeHttpConnectionPool\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-node-http-connection-pool-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualNodeHttpConnectionPool
---
