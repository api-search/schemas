---
description: An object that represents the current status of a route.
layout: schema
name: RouteStatus
properties_list:
- description: ''
  name: status
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-route-status-schema.json
slug: app-mesh-route-status
source_filename: app-mesh-route-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RouteStatusCode\"\n        },\n        {\n          \"description\": \"The current status for the route.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ],\n  \"description\": \"An object that represents the current status of a route.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-route-status-schema.json\",\n  \"title\": \"RouteStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-route-status-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: RouteStatus
---
