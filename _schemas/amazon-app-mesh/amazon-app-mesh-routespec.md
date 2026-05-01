---
description: An object that represents a route specification. Specify one route type.
layout: schema
name: RouteSpec
properties_list:
- description: ''
  name: grpcRoute
  type: object
- description: ''
  name: http2Route
  type: object
- description: ''
  name: httpRoute
  type: object
- description: ''
  name: priority
  type: object
- description: ''
  name: tcpRoute
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-routespec-schema.json
slug: amazon-app-mesh-routespec
source_filename: amazon-app-mesh-routespec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"RouteSpec\",\n  \"description\": \"An object that represents a route specification. Specify one route type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grpcRoute\": {},\n    \"http2Route\": {},\n    \"httpRoute\": {},\n    \"priority\": {},\n    \"tcpRoute\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-routespec-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: RouteSpec
---
