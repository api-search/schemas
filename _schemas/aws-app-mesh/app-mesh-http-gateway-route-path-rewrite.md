---
description: An object that represents the path to rewrite.
layout: schema
name: HttpGatewayRoutePathRewrite
properties_list:
- description: ''
  name: exact
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-gateway-route-path-rewrite-schema.json
slug: app-mesh-http-gateway-route-path-rewrite
source_filename: app-mesh-http-gateway-route-path-rewrite-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"exact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpPathExact\"\n        },\n        {\n          \"description\": \"The exact path to rewrite.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the path to rewrite.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-path-rewrite-schema.json\",\n  \"title\": \"HttpGatewayRoutePathRewrite\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-path-rewrite-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpGatewayRoutePathRewrite
---
