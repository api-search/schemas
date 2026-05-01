---
description: An object representing the beginning characters of the route to rewrite.
layout: schema
name: HttpGatewayRoutePrefixRewrite
properties_list:
- description: ''
  name: defaultPrefix
  type: object
- description: ''
  name: value
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-gateway-route-prefix-rewrite-schema.json
slug: app-mesh-http-gateway-route-prefix-rewrite
source_filename: app-mesh-http-gateway-route-prefix-rewrite-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultGatewayRouteRewrite\"\n        },\n        {\n          \"description\": \"The default prefix used to replace the incoming route prefix when rewritten.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpGatewayRoutePrefix\"\n        },\n        {\n          \"description\": \"The value used to replace the incoming route prefix when rewritten.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object representing the beginning characters of the route to rewrite.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-prefix-rewrite-schema.json\",\n  \"title\": \"HttpGatewayRoutePrefixRewrite\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-prefix-rewrite-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpGatewayRoutePrefixRewrite
---
