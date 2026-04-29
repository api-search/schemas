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
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-httpgatewayroutematch-schema.json
slug: amazon-app-mesh-httpgatewayroutematch
source_filename: amazon-app-mesh-httpgatewayroutematch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HttpGatewayRouteMatch\",\n  \"description\": \"An object that represents the criteria for determining a request match.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"headers\": {},\n    \"hostname\": {},\n    \"method\": {},\n    \"path\": {},\n    \"port\": {},\n    \"prefix\": {},\n    \"queryParameters\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-httpgatewayroutematch-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: HttpGatewayRouteMatch
---
