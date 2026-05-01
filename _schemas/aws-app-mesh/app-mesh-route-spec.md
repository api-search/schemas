---
description: An object that represents a route specification. Specify one route type.
layout: schema
name: RouteSpec
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
- description: ''
  name: tcpRoute
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-route-spec-schema.json
slug: app-mesh-route-spec
source_filename: app-mesh-route-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"grpcRoute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcRoute\"\n        },\n        {\n          \"description\": \"An object that represents the specification of a gRPC route.\"\n        }\n      ]\n    },\n    \"http2Route\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpRoute\"\n        },\n        {\n          \"description\": \"An object that represents the specification of an HTTP/2 route.\"\n        }\n      ]\n    },\n    \"httpRoute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpRoute\"\n        },\n        {\n          \"description\": \"An object that represents the specification of an HTTP route.\"\n        }\n      ]\n    },\n    \"priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoutePriority\"\n        },\n        {\n          \"description\": \"The priority\
  \ for the route. Routes are matched based on the specified value, where 0 is the highest priority.\"\n        }\n      ]\n    },\n    \"tcpRoute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TcpRoute\"\n        },\n        {\n          \"description\": \"An object that represents the specification of a TCP route.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents a route specification. Specify one route type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-route-spec-schema.json\",\n  \"title\": \"RouteSpec\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-route-spec-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: RouteSpec
---
