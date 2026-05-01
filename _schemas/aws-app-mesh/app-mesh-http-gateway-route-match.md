---
description: An object that represents the criteria for determining a request match.
layout: schema
name: HttpGatewayRouteMatch
properties_list:
- description: ''
  name: headers
  type: object
- description: ''
  name: hostname
  type: object
- description: ''
  name: method
  type: object
- description: ''
  name: path
  type: object
- description: ''
  name: port
  type: object
- description: ''
  name: prefix
  type: object
- description: ''
  name: queryParameters
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-gateway-route-match-schema.json
slug: app-mesh-http-gateway-route-match
source_filename: app-mesh-http-gateway-route-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"headers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpGatewayRouteHeaders\"\n        },\n        {\n          \"description\": \"The client request headers to match on.\"\n        }\n      ]\n    },\n    \"hostname\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteHostnameMatch\"\n        },\n        {\n          \"description\": \"The host name to match on.\"\n        }\n      ]\n    },\n    \"method\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpMethod\"\n        },\n        {\n          \"description\": \"The method to match on.\"\n        }\n      ]\n    },\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpPathMatch\"\n        },\n        {\n          \"description\": \"The path to match on.\"\n        }\n      ]\n    },\n    \"port\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/ListenerPort\"\n        },\n        {\n          \"description\": \"The port number to match on.\"\n        }\n      ]\n    },\n    \"prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Specifies the path to match requests with. This parameter must always start with <code>/</code>, which by itself matches all requests to the virtual service name. You can also match for path-based routing of requests. For example, if your virtual service name is <code>my-service.local</code> and you want the route to match requests to <code>my-service.local/metrics</code>, your prefix should be <code>/metrics</code>.\"\n        }\n      ]\n    },\n    \"queryParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpQueryParameters\"\n        },\n        {\n          \"description\": \"The query parameter to match\
  \ on.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the criteria for determining a request match.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-match-schema.json\",\n  \"title\": \"HttpGatewayRouteMatch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-gateway-route-match-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpGatewayRouteMatch
---
