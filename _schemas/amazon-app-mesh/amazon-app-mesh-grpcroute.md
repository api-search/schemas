---
description: An object that represents a gRPC route type.
layout: schema
name: GrpcRoute
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: match
  type: object
- description: ''
  name: retryPolicy
  type: object
- description: ''
  name: timeout
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-grpcroute-schema.json
slug: amazon-app-mesh-grpcroute
source_filename: amazon-app-mesh-grpcroute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GrpcRoute\",\n  \"description\": \"An object that represents a gRPC route type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {},\n    \"match\": {},\n    \"retryPolicy\": {},\n    \"timeout\": {}\n  },\n  \"required\": [\n    \"action\",\n    \"match\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-grpcroute-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: GrpcRoute
---
