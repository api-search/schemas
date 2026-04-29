---
description: An object that represents the status of a virtual router.
layout: schema
name: VirtualRouterStatus
properties_list:
- description: ''
  name: status
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-router-status-schema.json
slug: app-mesh-virtual-router-status
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualRouterStatusCode\"\n        },\n        {\n          \"description\": \"The current status of the virtual router.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ],\n  \"description\": \"An object that represents the status of a virtual router. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-status-schema.json\",\n  \"title\": \"VirtualRouterStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-status-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualRouterStatus
---
