---
description: An object that represents the provider for a virtual service.
layout: schema
name: VirtualServiceProvider
properties_list:
- description: ''
  name: virtualNode
  type: object
- description: ''
  name: virtualRouter
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-service-provider-schema.json
slug: app-mesh-virtual-service-provider
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualNode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualNodeServiceProvider\"\n        },\n        {\n          \"description\": \"The virtual node associated with a virtual service.\"\n        }\n      ]\n    },\n    \"virtualRouter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualRouterServiceProvider\"\n        },\n        {\n          \"description\": \"The virtual router associated with a virtual service.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the provider for a virtual service.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-service-provider-schema.json\",\n  \"title\": \"VirtualServiceProvider\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-service-provider-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualServiceProvider
---
