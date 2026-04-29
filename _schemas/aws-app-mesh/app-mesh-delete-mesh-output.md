---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: DeleteMeshOutput
properties_list:
- description: ''
  name: mesh
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-delete-mesh-output-schema.json
slug: app-mesh-delete-mesh-output
source_filename: app-mesh-delete-mesh-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"mesh\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MeshData\"\n        },\n        {\n          \"description\": \"The service mesh that was deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"mesh\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-delete-mesh-output-schema.json\",\n  \"title\": \"DeleteMeshOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-delete-mesh-output-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: DeleteMeshOutput
---
