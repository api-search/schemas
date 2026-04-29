---
description: DeleteGatewayRouteOutput schema from AWS App Mesh
layout: schema
name: DeleteGatewayRouteOutput
properties_list:
- description: ''
  name: gatewayRoute
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-delete-gateway-route-output-schema.json
slug: app-mesh-delete-gateway-route-output
source_filename: app-mesh-delete-gateway-route-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"gatewayRoute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteData\"\n        },\n        {\n          \"description\": \"The gateway route that was deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"gatewayRoute\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-delete-gateway-route-output-schema.json\",\n  \"title\": \"DeleteGatewayRouteOutput\",\n  \"description\": \"DeleteGatewayRouteOutput schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-delete-gateway-route-output-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: DeleteGatewayRouteOutput
---
