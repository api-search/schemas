---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: DeleteRouteOutput
properties_list:
- description: ''
  name: route
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-delete-route-output-schema.json
slug: app-mesh-delete-route-output
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"route\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RouteData\"\n        },\n        {\n          \"description\": \"The route that was deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"route\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-delete-route-output-schema.json\",\n  \"title\": \"DeleteRouteOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-delete-route-output-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: DeleteRouteOutput
---
