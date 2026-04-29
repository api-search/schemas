---
description: An object representing the gateway route to rewrite.
layout: schema
name: HttpGatewayRouteRewrite
properties_list:
- description: ''
  name: hostname
  type: object
- description: ''
  name: path
  type: object
- description: ''
  name: prefix
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-gateway-route-rewrite-schema.json
slug: app-mesh-http-gateway-route-rewrite
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostname\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteHostnameRewrite\"\n        },\n        {\n          \"description\": \"The host name to rewrite.\"\n        }\n      ]\n    },\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpGatewayRoutePathRewrite\"\n        },\n        {\n          \"description\": \"The path to rewrite.\"\n        }\n      ]\n    },\n    \"prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpGatewayRoutePrefixRewrite\"\n        },\n        {\n          \"description\": \"The specified beginning characters to rewrite.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object representing the gateway route to rewrite.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-rewrite-schema.json\"\
  ,\n  \"title\": \"HttpGatewayRouteRewrite\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-rewrite-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpGatewayRouteRewrite
---
