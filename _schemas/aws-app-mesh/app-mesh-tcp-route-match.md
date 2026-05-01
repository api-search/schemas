---
description: An object representing the TCP route to match.
layout: schema
name: TcpRouteMatch
properties_list:
- description: ''
  name: port
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-tcp-route-match-schema.json
slug: app-mesh-tcp-route-match
source_filename: app-mesh-tcp-route-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerPort\"\n        },\n        {\n          \"description\": \"The port number to match on.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object representing the TCP route to match.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tcp-route-match-schema.json\",\n  \"title\": \"TcpRouteMatch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tcp-route-match-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: TcpRouteMatch
---
