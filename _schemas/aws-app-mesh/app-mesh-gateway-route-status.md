---
description: An object that represents the current status of a gateway route.
layout: schema
name: GatewayRouteStatus
properties_list:
- description: ''
  name: status
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-gateway-route-status-schema.json
slug: app-mesh-gateway-route-status
source_filename: app-mesh-gateway-route-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteStatusCode\"\n        },\n        {\n          \"description\": \"The current status for the gateway route.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ],\n  \"description\": \"An object that represents the current status of a gateway route.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-status-schema.json\",\n  \"title\": \"GatewayRouteStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-status-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GatewayRouteStatus
---
