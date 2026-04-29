---
description: ListGatewayRoutesOutput schema from AWS App Mesh
layout: schema
name: ListGatewayRoutesOutput
properties_list:
- description: ''
  name: gatewayRoutes
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-list-gateway-routes-output-schema.json
slug: app-mesh-list-gateway-routes-output
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"gatewayRoutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteList\"\n        },\n        {\n          \"description\": \"The list of existing gateway routes for the specified service mesh and virtual gateway.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> value to include in a future <code>ListGatewayRoutes</code> request. When the results of a <code>ListGatewayRoutes</code> request exceed <code>limit</code>, you can use this value to retrieve the next page of results. This value is <code>null</code> when there are no more results to return.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"gatewayRoutes\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-list-gateway-routes-output-schema.json\"\
  ,\n  \"title\": \"ListGatewayRoutesOutput\",\n  \"description\": \"ListGatewayRoutesOutput schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-list-gateway-routes-output-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: ListGatewayRoutesOutput
---
