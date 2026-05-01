---
description: An object that represents a virtual gateway returned by a list operation.
layout: schema
name: VirtualGatewayRef
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: meshName
  type: object
- description: ''
  name: meshOwner
  type: object
- description: ''
  name: resourceOwner
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: virtualGatewayName
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualgatewayref-schema.json
slug: amazon-app-mesh-virtualgatewayref
source_filename: amazon-app-mesh-virtualgatewayref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualGatewayRef\",\n  \"description\": \"An object that represents a virtual gateway returned by a list operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {},\n    \"createdAt\": {},\n    \"lastUpdatedAt\": {},\n    \"meshName\": {},\n    \"meshOwner\": {},\n    \"resourceOwner\": {},\n    \"version\": {},\n    \"virtualGatewayName\": {}\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"lastUpdatedAt\",\n    \"meshName\",\n    \"meshOwner\",\n    \"resourceOwner\",\n    \"version\",\n    \"virtualGatewayName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualgatewayref-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayRef
---
