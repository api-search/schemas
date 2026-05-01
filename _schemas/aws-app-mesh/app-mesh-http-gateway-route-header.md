---
description: An object that represents the HTTP header in the gateway route.
layout: schema
name: HttpGatewayRouteHeader
properties_list:
- description: ''
  name: invert
  type: object
- description: ''
  name: match
  type: object
- description: ''
  name: name
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-gateway-route-header-schema.json
slug: app-mesh-http-gateway-route-header
source_filename: app-mesh-http-gateway-route-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"invert\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specify <code>True</code> to match anything except the match criteria. The default value is <code>False</code>.\"\n        }\n      ]\n    },\n    \"match\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderMatchMethod\"\n        },\n        {\n          \"description\": \"An object that represents the method and value to match with the header value sent in a request. Specify one match method.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderName\"\n        },\n        {\n          \"description\": \"A name for the HTTP header in the gateway route that will be matched on.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"description\"\
  : \"An object that represents the HTTP header in the gateway route.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-header-schema.json\",\n  \"title\": \"HttpGatewayRouteHeader\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-header-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpGatewayRouteHeader
---
