---
description: An object that represents the specification of a virtual router.
layout: schema
name: VirtualRouterSpec
properties_list:
- description: ''
  name: listeners
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-router-spec-schema.json
slug: app-mesh-virtual-router-spec
source_filename: app-mesh-virtual-router-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"listeners\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualRouterListeners\"\n        },\n        {\n          \"description\": \"The listeners that the virtual router is expected to receive inbound traffic from. You can specify one listener.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the specification of a virtual router.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-spec-schema.json\",\n  \"title\": \"VirtualRouterSpec\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-spec-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualRouterSpec
---
