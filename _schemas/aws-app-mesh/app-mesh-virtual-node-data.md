---
description: An object that represents a virtual node returned by a describe operation.
layout: schema
name: VirtualNodeData
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
  name: virtualNodeName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-node-data-schema.json
slug: app-mesh-virtual-node-data
source_filename: app-mesh-virtual-node-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"meshName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service mesh that the virtual node resides in.\"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceMetadata\"\n        },\n        {\n          \"description\": \"The associated metadata for the virtual node.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualNodeSpec\"\n        },\n        {\n          \"description\": \"The specifications of the virtual node.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualNodeStatus\"\n        },\n        {\n          \"description\": \"The current status for the virtual node.\"\
  \n        }\n      ]\n    },\n    \"virtualNodeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the virtual node.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"meshName\",\n    \"metadata\",\n    \"spec\",\n    \"status\",\n    \"virtualNodeName\"\n  ],\n  \"description\": \"An object that represents a virtual node returned by a describe operation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-node-data-schema.json\",\n  \"title\": \"VirtualNodeData\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-node-data-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualNodeData
---
