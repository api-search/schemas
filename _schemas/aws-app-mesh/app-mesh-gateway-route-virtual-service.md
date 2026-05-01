---
description: An object that represents the virtual service that traffic is routed to.
layout: schema
name: GatewayRouteVirtualService
properties_list:
- description: ''
  name: virtualServiceName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-gateway-route-virtual-service-schema.json
slug: app-mesh-gateway-route-virtual-service
source_filename: app-mesh-gateway-route-virtual-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the virtual service that traffic is routed to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualServiceName\"\n  ],\n  \"description\": \"An object that represents the virtual service that traffic is routed to.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-virtual-service-schema.json\",\n  \"title\": \"GatewayRouteVirtualService\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-virtual-service-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GatewayRouteVirtualService
---
