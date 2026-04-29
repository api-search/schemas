---
description: An object that represents the gateway route to rewrite.
layout: schema
name: GrpcGatewayRouteRewrite
properties_list:
- description: ''
  name: hostname
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-gateway-route-rewrite-schema.json
slug: app-mesh-grpc-gateway-route-rewrite
source_filename: app-mesh-grpc-gateway-route-rewrite-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostname\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteHostnameRewrite\"\n        },\n        {\n          \"description\": \"The host name of the gateway route to rewrite.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the gateway route to rewrite.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-gateway-route-rewrite-schema.json\",\n  \"title\": \"GrpcGatewayRouteRewrite\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-gateway-route-rewrite-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcGatewayRouteRewrite
---
