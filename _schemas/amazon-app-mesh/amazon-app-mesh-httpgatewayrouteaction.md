---
description: An object that represents the action to take if a match is determined.
layout: schema
name: HttpGatewayRouteAction
properties_list:
- description: ''
  name: rewrite
  type: object
- description: ''
  name: target
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-httpgatewayrouteaction-schema.json
slug: amazon-app-mesh-httpgatewayrouteaction
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HttpGatewayRouteAction\",\n  \"description\": \"An object that represents the action to take if a match is determined.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rewrite\": {},\n    \"target\": {}\n  },\n  \"required\": [\n    \"target\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-httpgatewayrouteaction-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: HttpGatewayRouteAction
---
