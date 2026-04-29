---
description: An object that represents a service mesh returned by a describe operation.
layout: schema
name: MeshData
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
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-mesh-data-schema.json
slug: app-mesh-mesh-data
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"meshName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service mesh.\"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceMetadata\"\n        },\n        {\n          \"description\": \"The associated metadata for the service mesh.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MeshSpec\"\n        },\n        {\n          \"description\": \"The associated specification for the service mesh.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MeshStatus\"\n        },\n        {\n          \"description\": \"The status of the service mesh.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"meshName\",\n    \"metadata\",\n    \"spec\",\n    \"status\"\n  ],\n  \"description\": \"An object that represents a service mesh returned by a describe operation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-mesh-data-schema.json\",\n  \"title\": \"MeshData\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-mesh-data-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: MeshData
---
