---
description: An object that represents the action to take if a match is determined.
layout: schema
name: TcpRouteAction
properties_list:
- description: ''
  name: weightedTargets
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-tcp-route-action-schema.json
slug: app-mesh-tcp-route-action
source_filename: app-mesh-tcp-route-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"weightedTargets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WeightedTargets\"\n        },\n        {\n          \"description\": \"An object that represents the targets that traffic is routed to when a request matches the route.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"weightedTargets\"\n  ],\n  \"description\": \"An object that represents the action to take if a match is determined.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tcp-route-action-schema.json\",\n  \"title\": \"TcpRouteAction\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tcp-route-action-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: TcpRouteAction
---
