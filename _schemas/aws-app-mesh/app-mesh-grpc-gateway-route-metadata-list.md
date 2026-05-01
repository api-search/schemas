---
description: GrpcGatewayRouteMetadataList schema from AWS App Mesh
layout: schema
name: GrpcGatewayRouteMetadataList
properties_list: []
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-gateway-route-metadata-list-schema.json
slug: app-mesh-grpc-gateway-route-metadata-list
source_filename: app-mesh-grpc-gateway-route-metadata-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"invert\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"Specify <code>True</code> to match anything except the match criteria. The default value is <code>False</code>.\"\n          }\n        ]\n      },\n      \"match\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/GrpcMetadataMatchMethod\"\n          },\n          {\n            \"description\": \"The criteria for determining a metadata match.\"\n          }\n        ]\n      },\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/HeaderName\"\n          },\n          {\n            \"description\": \"A name for the gateway route metadata.\"\n          }\n        ]\n      }\n    },\n    \"required\": [\n      \"name\"\n    ],\n    \"description\"\
  : \"An object representing the metadata of the gateway route.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-gateway-route-metadata-list-schema.json\",\n  \"title\": \"GrpcGatewayRouteMetadataList\",\n  \"description\": \"GrpcGatewayRouteMetadataList schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-gateway-route-metadata-list-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcGatewayRouteMetadataList
---
