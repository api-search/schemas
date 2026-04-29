---
description: ''
layout: schema
name: CreateVirtualGatewayInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: virtualGatewayName
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-createvirtualgatewayinput-schema.json
slug: amazon-app-mesh-createvirtualgatewayinput
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateVirtualGatewayInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {},\n    \"spec\": {},\n    \"tags\": {},\n    \"virtualGatewayName\": {}\n  },\n  \"required\": [\n    \"spec\",\n    \"virtualGatewayName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-createvirtualgatewayinput-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: CreateVirtualGatewayInput
---
