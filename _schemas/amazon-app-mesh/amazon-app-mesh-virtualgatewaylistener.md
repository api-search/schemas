---
description: An object that represents a listener for a virtual gateway.
layout: schema
name: VirtualGatewayListener
properties_list:
- description: ''
  name: connectionPool
  type: object
- description: ''
  name: healthCheck
  type: object
- description: ''
  name: portMapping
  type: object
- description: ''
  name: tls
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualgatewaylistener-schema.json
slug: amazon-app-mesh-virtualgatewaylistener
source_filename: amazon-app-mesh-virtualgatewaylistener-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualGatewayListener\",\n  \"description\": \"An object that represents a listener for a virtual gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionPool\": {},\n    \"healthCheck\": {},\n    \"portMapping\": {},\n    \"tls\": {}\n  },\n  \"required\": [\n    \"portMapping\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualgatewaylistener-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayListener
---
