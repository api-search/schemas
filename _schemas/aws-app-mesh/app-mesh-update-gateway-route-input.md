---
description: UpdateGatewayRouteInput schema from AWS App Mesh
layout: schema
name: UpdateGatewayRouteInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: spec
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-update-gateway-route-input-schema.json
slug: app-mesh-update-gateway-route-input
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request. Up to 36 letters, numbers, hyphens, and underscores are allowed.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteSpec\"\n        },\n        {\n          \"description\": \"The new gateway route specification to apply. This overwrites the existing data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"spec\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-update-gateway-route-input-schema.json\",\n  \"title\": \"UpdateGatewayRouteInput\",\n  \"description\"\
  : \"UpdateGatewayRouteInput schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-update-gateway-route-input-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: UpdateGatewayRouteInput
---
