---
description: An object that represents an HTTP gateway route.
layout: schema
name: HttpGatewayRoute
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: match
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-gateway-route-schema.json
slug: app-mesh-http-gateway-route
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpGatewayRouteAction\"\n        },\n        {\n          \"description\": \"An object that represents the action to take if a match is determined.\"\n        }\n      ]\n    },\n    \"match\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpGatewayRouteMatch\"\n        },\n        {\n          \"description\": \"An object that represents the criteria for determining a request match.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"action\",\n    \"match\"\n  ],\n  \"description\": \"An object that represents an HTTP gateway route.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-schema.json\",\n  \"title\": \"HttpGatewayRoute\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpGatewayRoute
---
