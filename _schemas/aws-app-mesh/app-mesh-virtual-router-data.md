---
description: An object that represents a virtual router returned by a describe operation.
layout: schema
name: VirtualRouterData
properties_list:
- description: ''
  name: meshName
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: virtualRouterName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-router-data-schema.json
slug: app-mesh-virtual-router-data
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"meshName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service mesh that the virtual router resides in.\"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceMetadata\"\n        },\n        {\n          \"description\": \"The associated metadata for the virtual router.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualRouterSpec\"\n        },\n        {\n          \"description\": \"The specifications of the virtual router.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualRouterStatus\"\n        },\n        {\n          \"description\": \"The current status of the virtual\
  \ router.\"\n        }\n      ]\n    },\n    \"virtualRouterName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the virtual router.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"meshName\",\n    \"metadata\",\n    \"spec\",\n    \"status\",\n    \"virtualRouterName\"\n  ],\n  \"description\": \"An object that represents a virtual router returned by a describe operation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-data-schema.json\",\n  \"title\": \"VirtualRouterData\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-data-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualRouterData
---
