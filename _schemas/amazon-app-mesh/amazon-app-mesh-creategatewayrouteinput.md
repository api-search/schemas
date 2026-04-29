---
description: ''
layout: schema
name: CreateGatewayRouteInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: gatewayRouteName
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-creategatewayrouteinput-schema.json
slug: amazon-app-mesh-creategatewayrouteinput
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateGatewayRouteInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {},\n    \"gatewayRouteName\": {},\n    \"spec\": {},\n    \"tags\": {}\n  },\n  \"required\": [\n    \"gatewayRouteName\",\n    \"spec\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-creategatewayrouteinput-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: CreateGatewayRouteInput
---
