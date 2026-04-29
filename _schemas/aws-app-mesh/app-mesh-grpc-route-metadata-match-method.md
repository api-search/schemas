---
description: An object that represents the match method. Specify one of the match values.
layout: schema
name: GrpcRouteMetadataMatchMethod
properties_list:
- description: ''
  name: exact
  type: object
- description: ''
  name: prefix
  type: object
- description: ''
  name: range
  type: object
- description: ''
  name: regex
  type: object
- description: ''
  name: suffix
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-route-metadata-match-method-schema.json
slug: app-mesh-grpc-route-metadata-match-method
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"exact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderMatch\"\n        },\n        {\n          \"description\": \"The value sent by the client must match the specified value exactly.\"\n        }\n      ]\n    },\n    \"prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderMatch\"\n        },\n        {\n          \"description\": \"The value sent by the client must begin with the specified characters.\"\n        }\n      ]\n    },\n    \"range\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchRange\"\n        },\n        {\n          \"description\": \"An object that represents the range of values to match on.\"\n        }\n      ]\n    },\n    \"regex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderMatch\"\n        },\n        {\n          \"description\": \"The value sent\
  \ by the client must include the specified characters.\"\n        }\n      ]\n    },\n    \"suffix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderMatch\"\n        },\n        {\n          \"description\": \"The value sent by the client must end with the specified characters.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the match method. Specify one of the match values.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-route-metadata-match-method-schema.json\",\n  \"title\": \"GrpcRouteMetadataMatchMethod\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-route-metadata-match-method-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcRouteMetadataMatchMethod
---
