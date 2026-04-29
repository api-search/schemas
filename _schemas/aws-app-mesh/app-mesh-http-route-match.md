---
description: An object that represents the requirements for a route to match HTTP requests for a virtual router.
layout: schema
name: HttpRouteMatch
properties_list:
- description: ''
  name: headers
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
- description: ''
  name: scheme
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-route-match-schema.json
slug: app-mesh-http-route-match
source_filename: app-mesh-http-route-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"headers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpRouteHeaders\"\n        },\n        {\n          \"description\": \"The client request headers to match on.\"\n        }\n      ]\n    },\n    \"method\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpMethod\"\n        },\n        {\n          \"description\": \"The client request method to match on. Specify only one.\"\n        }\n      ]\n    },\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpPathMatch\"\n        },\n        {\n          \"description\": \"The client request path to match on.\"\n        }\n      ]\n    },\n    \"port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerPort\"\n        },\n        {\n          \"description\": \"The port number to match on.\"\n        }\n      ]\n    },\n    \"prefix\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Specifies the path to match requests with. This parameter must always start with <code>/</code>, which by itself matches all requests to the virtual service name. You can also match for path-based routing of requests. For example, if your virtual service name is <code>my-service.local</code> and you want the route to match requests to <code>my-service.local/metrics</code>, your prefix should be <code>/metrics</code>.\"\n        }\n      ]\n    },\n    \"queryParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpQueryParameters\"\n        },\n        {\n          \"description\": \"The client request query parameters to match on.\"\n        }\n      ]\n    },\n    \"scheme\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpScheme\"\n        },\n        {\n          \"description\"\
  : \"The client request scheme to match on. Specify only one. Applicable only for HTTP2 routes.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the requirements for a route to match HTTP requests for a virtual router.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-route-match-schema.json\",\n  \"title\": \"HttpRouteMatch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-route-match-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpRouteMatch
---
