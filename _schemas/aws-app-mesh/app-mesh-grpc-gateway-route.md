---
description: An object that represents a gRPC gateway route.
layout: schema
name: GrpcGatewayRoute
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: match
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-gateway-route-schema.json
slug: app-mesh-grpc-gateway-route
source_filename: app-mesh-grpc-gateway-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcGatewayRouteAction\"\n        },\n        {\n          \"description\": \"An object that represents the action to take if a match is determined.\"\n        }\n      ]\n    },\n    \"match\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcGatewayRouteMatch\"\n        },\n        {\n          \"description\": \"An object that represents the criteria for determining a request match.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"action\",\n    \"match\"\n  ],\n  \"description\": \"An object that represents a gRPC gateway route.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-gateway-route-schema.json\",\n  \"title\": \"GrpcGatewayRoute\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-gateway-route-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcGatewayRoute
---
