---
description: CreateGatewayRouteInput schema from AWS App Mesh
layout: schema
name: CreateGatewayRouteInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: gatewayRouteName
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: tags
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-create-gateway-route-input-schema.json
slug: app-mesh-create-gateway-route-input
source_filename: app-mesh-create-gateway-route-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request. Up to 36 letters, numbers, hyphens, and underscores are allowed.\"\n        }\n      ]\n    },\n    \"gatewayRouteName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name to use for the gateway route.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteSpec\"\n        },\n        {\n          \"description\": \"The gateway route specification to apply.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n\
  \        {\n          \"description\": \"Optional metadata that you can apply to the gateway route to assist with categorization and organization. Each tag consists of a key and an optional value, both of which you define. Tag keys can have a maximum character length of 128 characters, and tag values can have a maximum length of 256 characters.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"gatewayRouteName\",\n    \"spec\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-create-gateway-route-input-schema.json\",\n  \"title\": \"CreateGatewayRouteInput\",\n  \"description\": \"CreateGatewayRouteInput schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-create-gateway-route-input-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: CreateGatewayRouteInput
---
