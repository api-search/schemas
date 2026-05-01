---
description: An object that represents the default properties for a backend.
layout: schema
name: VirtualGatewayBackendDefaults
properties_list:
- description: ''
  name: clientPolicy
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-backend-defaults-schema.json
slug: app-mesh-virtual-gateway-backend-defaults
source_filename: app-mesh-virtual-gateway-backend-defaults-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayClientPolicy\"\n        },\n        {\n          \"description\": \"A reference to an object that represents a client policy.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the default properties for a backend.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-backend-defaults-schema.json\",\n  \"title\": \"VirtualGatewayBackendDefaults\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-backend-defaults-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayBackendDefaults
---
