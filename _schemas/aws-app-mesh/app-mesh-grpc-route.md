---
description: An object that represents a gRPC route type.
layout: schema
name: GrpcRoute
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: match
  type: object
- description: ''
  name: retryPolicy
  type: object
- description: ''
  name: timeout
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-route-schema.json
slug: app-mesh-grpc-route
source_filename: app-mesh-grpc-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcRouteAction\"\n        },\n        {\n          \"description\": \"An object that represents the action to take if a match is determined.\"\n        }\n      ]\n    },\n    \"match\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcRouteMatch\"\n        },\n        {\n          \"description\": \"An object that represents the criteria for determining a request match.\"\n        }\n      ]\n    },\n    \"retryPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcRetryPolicy\"\n        },\n        {\n          \"description\": \"An object that represents a retry policy.\"\n        }\n      ]\n    },\n    \"timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcTimeout\"\n        },\n        {\n          \"description\": \"An object\
  \ that represents types of timeouts. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"action\",\n    \"match\"\n  ],\n  \"description\": \"An object that represents a gRPC route type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-route-schema.json\",\n  \"title\": \"GrpcRoute\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-route-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcRoute
---
