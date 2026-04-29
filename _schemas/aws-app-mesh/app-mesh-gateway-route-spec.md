---
description: An object that represents a gateway route specification. Specify one gateway route type.
layout: schema
name: GatewayRouteSpec
properties_list:
- description: ''
  name: grpcRoute
  type: object
- description: ''
  name: http2Route
  type: object
- description: ''
  name: httpRoute
  type: object
- description: ''
  name: priority
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-gateway-route-spec-schema.json
slug: app-mesh-gateway-route-spec
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"grpcRoute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcGatewayRoute\"\n        },\n        {\n          \"description\": \"An object that represents the specification of a gRPC gateway route.\"\n        }\n      ]\n    },\n    \"http2Route\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpGatewayRoute\"\n        },\n        {\n          \"description\": \"An object that represents the specification of an HTTP/2 gateway route.\"\n        }\n      ]\n    },\n    \"httpRoute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpGatewayRoute\"\n        },\n        {\n          \"description\": \"An object that represents the specification of an HTTP gateway route.\"\n        }\n      ]\n    },\n    \"priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRoutePriority\"\n        },\n\
  \        {\n          \"description\": \"The ordering of the gateway routes spec.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents a gateway route specification. Specify one gateway route type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-spec-schema.json\",\n  \"title\": \"GatewayRouteSpec\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-spec-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GatewayRouteSpec
---
