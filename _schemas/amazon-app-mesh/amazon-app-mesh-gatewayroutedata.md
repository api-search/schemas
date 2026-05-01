---
description: An object that represents a gateway route returned by a describe operation.
layout: schema
name: GatewayRouteData
properties_list:
- description: ''
  name: gatewayRouteName
  type: object
- description: ''
  name: meshName
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: virtualGatewayName
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-gatewayroutedata-schema.json
slug: amazon-app-mesh-gatewayroutedata
source_filename: amazon-app-mesh-gatewayroutedata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GatewayRouteData\",\n  \"description\": \"An object that represents a gateway route returned by a describe operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gatewayRouteName\": {},\n    \"meshName\": {},\n    \"metadata\": {\n      \"$ref\": \"#/definitions/ResourceMetadata\"\n    },\n    \"spec\": {},\n    \"status\": {},\n    \"virtualGatewayName\": {}\n  },\n  \"required\": [\n    \"gatewayRouteName\",\n    \"meshName\",\n    \"metadata\",\n    \"spec\",\n    \"status\",\n    \"virtualGatewayName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-gatewayroutedata-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: GatewayRouteData
---
