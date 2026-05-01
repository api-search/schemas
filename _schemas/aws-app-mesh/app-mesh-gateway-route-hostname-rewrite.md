---
description: An object representing the gateway route host name to rewrite.
layout: schema
name: GatewayRouteHostnameRewrite
properties_list:
- description: ''
  name: defaultTargetHostname
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-gateway-route-hostname-rewrite-schema.json
slug: app-mesh-gateway-route-hostname-rewrite
source_filename: app-mesh-gateway-route-hostname-rewrite-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultTargetHostname\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultGatewayRouteRewrite\"\n        },\n        {\n          \"description\": \"The default target host name to write to.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object representing the gateway route host name to rewrite.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-hostname-rewrite-schema.json\",\n  \"title\": \"GatewayRouteHostnameRewrite\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-hostname-rewrite-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GatewayRouteHostnameRewrite
---
