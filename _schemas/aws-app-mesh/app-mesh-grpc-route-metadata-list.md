---
description: GrpcRouteMetadataList schema from AWS App Mesh
layout: schema
name: GrpcRouteMetadataList
properties_list: []
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-route-metadata-list-schema.json
slug: app-mesh-grpc-route-metadata-list
source_filename: app-mesh-grpc-route-metadata-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"invert\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"Specify <code>True</code> to match anything except the match criteria. The default value is <code>False</code>.\"\n          }\n        ]\n      },\n      \"match\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/GrpcRouteMetadataMatchMethod\"\n          },\n          {\n            \"description\": \"An object that represents the data to match from the request.\"\n          }\n        ]\n      },\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/HeaderName\"\n          },\n          {\n            \"description\": \"The name of the route.\"\n          }\n        ]\n      }\n    },\n    \"required\": [\n      \"name\"\n    ],\n   \
  \ \"description\": \"An object that represents the match metadata for the route.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-route-metadata-list-schema.json\",\n  \"title\": \"GrpcRouteMetadataList\",\n  \"description\": \"GrpcRouteMetadataList schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-route-metadata-list-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcRouteMetadataList
---
