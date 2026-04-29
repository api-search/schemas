---
description: An object representing the metadata of the gateway route.
layout: schema
name: GrpcGatewayRouteMetadata
properties_list:
- description: ''
  name: invert
  type: object
- description: ''
  name: match
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-grpcgatewayroutemetadata-schema.json
slug: amazon-app-mesh-grpcgatewayroutemetadata
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GrpcGatewayRouteMetadata\",\n  \"description\": \"An object representing the metadata of the gateway route.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invert\": {},\n    \"match\": {},\n    \"name\": {}\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-grpcgatewayroutemetadata-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: GrpcGatewayRouteMetadata
---
