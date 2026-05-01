---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: CreateRouteOutput
properties_list:
- description: ''
  name: route
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-create-route-output-schema.json
slug: app-mesh-create-route-output
source_filename: app-mesh-create-route-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"route\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RouteData\"\n        },\n        {\n          \"description\": \"The full description of your mesh following the create call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"route\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-create-route-output-schema.json\",\n  \"title\": \"CreateRouteOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-create-route-output-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: CreateRouteOutput
---
