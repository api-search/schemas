---
description: An object that represents the specification of a service mesh resource.
layout: schema
name: VirtualGatewaySpec
properties_list:
- description: ''
  name: backendDefaults
  type: object
- description: ''
  name: listeners
  type: object
- description: ''
  name: logging
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualgatewayspec-schema.json
slug: amazon-app-mesh-virtualgatewayspec
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualGatewaySpec\",\n  \"description\": \"An object that represents the specification of a service mesh resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"backendDefaults\": {},\n    \"listeners\": {},\n    \"logging\": {\n      \"$ref\": \"#/definitions/VirtualGatewayLogging\"\n    }\n  },\n  \"required\": [\n    \"listeners\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualgatewayspec-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: VirtualGatewaySpec
---
