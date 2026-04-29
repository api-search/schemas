---
description: An object that represents the current status of the virtual node.
layout: schema
name: VirtualNodeStatus
properties_list:
- description: ''
  name: status
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-node-status-schema.json
slug: app-mesh-virtual-node-status
source_filename: app-mesh-virtual-node-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualNodeStatusCode\"\n        },\n        {\n          \"description\": \"The current status of the virtual node.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ],\n  \"description\": \"An object that represents the current status of the virtual node.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-node-status-schema.json\",\n  \"title\": \"VirtualNodeStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-node-status-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualNodeStatus
---
