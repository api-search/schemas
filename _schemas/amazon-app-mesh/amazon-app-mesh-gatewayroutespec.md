---
description: An object that represents a gateway route specification. Specify one gateway route type.
layout: schema
name: GatewayRouteSpec
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
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-gatewayroutespec-schema.json
slug: amazon-app-mesh-gatewayroutespec
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GatewayRouteSpec\",\n  \"description\": \"An object that represents a gateway route specification. Specify one gateway route type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grpcRoute\": {},\n    \"http2Route\": {},\n    \"httpRoute\": {},\n    \"priority\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-gatewayroutespec-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: GatewayRouteSpec
---
