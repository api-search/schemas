---
description: An object that represents a gateway route target.
layout: schema
name: GatewayRouteTarget
properties_list:
- description: ''
  name: port
  type: object
- description: ''
  name: virtualService
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-gatewayroutetarget-schema.json
slug: amazon-app-mesh-gatewayroutetarget
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GatewayRouteTarget\",\n  \"description\": \"An object that represents a gateway route target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"port\": {},\n    \"virtualService\": {}\n  },\n  \"required\": [\n    \"virtualService\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-gatewayroutetarget-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: GatewayRouteTarget
---
