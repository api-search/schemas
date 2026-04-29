---
description: VirtualRouterListeners schema from AWS App Mesh
layout: schema
name: VirtualRouterListeners
properties_list: []
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-router-listeners-schema.json
slug: app-mesh-virtual-router-listeners
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"portMapping\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"port\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/PortNumber\"\n              },\n              {\n                \"description\": \"The port used for the port mapping.\"\n              }\n            ]\n          },\n          \"protocol\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/PortProtocol\"\n              },\n              {\n                \"description\": \"The protocol used for the port mapping. Specify one protocol.\"\n              }\n            ]\n          }\n        },\n        \"required\": [\n          \"port\",\n          \"protocol\"\n        ],\n        \"description\": \"An object that represents a port mapping.\"\n      }\n    },\n    \"required\": [\n      \"\
  portMapping\"\n    ],\n    \"description\": \"An object that represents a virtual router listener.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-listeners-schema.json\",\n  \"title\": \"VirtualRouterListeners\",\n  \"description\": \"VirtualRouterListeners schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-listeners-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualRouterListeners
---
