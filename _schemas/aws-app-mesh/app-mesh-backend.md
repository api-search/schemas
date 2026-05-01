---
description: An object that represents the backends that a virtual node is expected to send outbound traffic to.
layout: schema
name: Backend
properties_list:
- description: ''
  name: virtualService
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-backend-schema.json
slug: app-mesh-backend
source_filename: app-mesh-backend-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualService\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualServiceBackend\"\n        },\n        {\n          \"description\": \"Specifies a virtual service to use as a backend. \"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the backends that a virtual node is expected to send outbound traffic to.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-backend-schema.json\",\n  \"title\": \"Backend\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-backend-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: Backend
---
