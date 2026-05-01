---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: UpdateMeshOutput
properties_list:
- description: An object that represents a service mesh returned by a describe operation.
  name: mesh
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-update-mesh-output-schema.json
slug: app-mesh-update-mesh-output
source_filename: app-mesh-update-mesh-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"mesh\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"meshName\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ResourceName\"\n            },\n            {\n              \"description\": \"The name of the service mesh.\"\n            }\n          ]\n        },\n        \"metadata\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ResourceMetadata\"\n            },\n            {\n              \"description\": \"The associated metadata for the service mesh.\"\n            }\n          ]\n        },\n        \"spec\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/MeshSpec\"\n            },\n            {\n              \"description\": \"The associated specification for the service mesh.\"\n            }\n          ]\n        },\n        \"status\": {\n          \"allOf\"\
  : [\n            {\n              \"$ref\": \"#/components/schemas/MeshStatus\"\n            },\n            {\n              \"description\": \"The status of the service mesh.\"\n            }\n          ]\n        }\n      },\n      \"required\": [\n        \"meshName\",\n        \"metadata\",\n        \"spec\",\n        \"status\"\n      ],\n      \"description\": \"An object that represents a service mesh returned by a describe operation.\"\n    }\n  },\n  \"required\": [\n    \"mesh\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-update-mesh-output-schema.json\",\n  \"title\": \"UpdateMeshOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-update-mesh-output-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: UpdateMeshOutput
---
