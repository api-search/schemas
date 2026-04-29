---
description: Backends schema from AWS App Mesh
layout: schema
name: Backends
properties_list: []
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-backends-schema.json
slug: app-mesh-backends
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"virtualService\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/VirtualServiceBackend\"\n          },\n          {\n            \"description\": \"Specifies a virtual service to use as a backend. \"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that represents the backends that a virtual node is expected to send outbound traffic to.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-backends-schema.json\",\n  \"title\": \"Backends\",\n  \"description\": \"Backends schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-backends-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: Backends
---
