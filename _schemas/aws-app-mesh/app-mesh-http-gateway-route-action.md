---
description: An object that represents the action to take if a match is determined.
layout: schema
name: HttpGatewayRouteAction
properties_list:
- description: ''
  name: rewrite
  type: object
- description: ''
  name: target
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-gateway-route-action-schema.json
slug: app-mesh-http-gateway-route-action
source_filename: app-mesh-http-gateway-route-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"rewrite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpGatewayRouteRewrite\"\n        },\n        {\n          \"description\": \"The gateway route action to rewrite.\"\n        }\n      ]\n    },\n    \"target\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteTarget\"\n        },\n        {\n          \"description\": \"An object that represents the target that traffic is routed to when a request matches the gateway route.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"target\"\n  ],\n  \"description\": \"An object that represents the action to take if a match is determined.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-action-schema.json\",\n  \"title\": \"HttpGatewayRouteAction\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-action-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpGatewayRouteAction
---
