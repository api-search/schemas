---
description: An object that represents a type of connection pool.
layout: schema
name: VirtualNodeTcpConnectionPool
properties_list:
- description: ''
  name: maxConnections
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-node-tcp-connection-pool-schema.json
slug: app-mesh-virtual-node-tcp-connection-pool
source_filename: app-mesh-virtual-node-tcp-connection-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxConnections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxConnections\"\n        },\n        {\n          \"description\": \"Maximum number of outbound TCP connections Envoy can establish concurrently with all hosts in upstream cluster.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"maxConnections\"\n  ],\n  \"description\": \"An object that represents a type of connection pool.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-node-tcp-connection-pool-schema.json\",\n  \"title\": \"VirtualNodeTcpConnectionPool\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-node-tcp-connection-pool-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualNodeTcpConnectionPool
---
