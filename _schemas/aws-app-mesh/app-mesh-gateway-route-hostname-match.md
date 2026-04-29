---
description: An object representing the gateway route host name to match.
layout: schema
name: GatewayRouteHostnameMatch
properties_list:
- description: ''
  name: exact
  type: object
- description: ''
  name: suffix
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-gateway-route-hostname-match-schema.json
slug: app-mesh-gateway-route-hostname-match
source_filename: app-mesh-gateway-route-hostname-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"exact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExactHostName\"\n        },\n        {\n          \"description\": \"The exact host name to match on.\"\n        }\n      ]\n    },\n    \"suffix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SuffixHostname\"\n        },\n        {\n          \"description\": \"The specified ending characters of the host name to match on.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object representing the gateway route host name to match.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-hostname-match-schema.json\",\n  \"title\": \"GatewayRouteHostnameMatch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-gateway-route-hostname-match-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GatewayRouteHostnameMatch
---
