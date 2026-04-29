---
description: An object that represents a gateway route target.
layout: schema
name: GatewayRouteTarget
properties_list:
- description: ''
  name: port
  type: object
- description: ''
  name: virtualService
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-gateway-route-target-schema.json
slug: app-mesh-gateway-route-target
source_filename: app-mesh-gateway-route-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerPort\"\n        },\n        {\n          \"description\": \"The port number of the gateway route target.\"\n        }\n      ]\n    },\n    \"virtualService\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteVirtualService\"\n        },\n        {\n          \"description\": \"An object that represents a virtual service gateway route target.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualService\"\n  ],\n  \"description\": \"An object that represents a gateway route target.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-target-schema.json\",\n  \"title\": \"GatewayRouteTarget\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-target-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GatewayRouteTarget
---
