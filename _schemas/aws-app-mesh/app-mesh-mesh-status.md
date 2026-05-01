---
description: An object that represents the status of a service mesh.
layout: schema
name: MeshStatus
properties_list:
- description: ''
  name: status
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-mesh-status-schema.json
slug: app-mesh-mesh-status
source_filename: app-mesh-mesh-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MeshStatusCode\"\n        },\n        {\n          \"description\": \"The current mesh status.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the status of a service mesh.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-mesh-status-schema.json\",\n  \"title\": \"MeshStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-mesh-status-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: MeshStatus
---
