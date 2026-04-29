---
description: An object that represents the match metadata for the route.
layout: schema
name: GrpcRouteMetadata
properties_list:
- description: ''
  name: invert
  type: object
- description: ''
  name: match
  type: object
- description: ''
  name: name
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-route-metadata-schema.json
slug: app-mesh-grpc-route-metadata
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"invert\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specify <code>True</code> to match anything except the match criteria. The default value is <code>False</code>.\"\n        }\n      ]\n    },\n    \"match\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcRouteMetadataMatchMethod\"\n        },\n        {\n          \"description\": \"An object that represents the data to match from the request.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderName\"\n        },\n        {\n          \"description\": \"The name of the route.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"description\": \"An object that represents the match metadata for the route.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-route-metadata-schema.json\",\n  \"title\": \"GrpcRouteMetadata\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-route-metadata-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcRouteMetadata
---
