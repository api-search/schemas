---
description: An object that represents the match metadata for the route.
layout: schema
name: GrpcRouteMetadata
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
schema_file: json-schema/amazon-app-mesh-grpcroutemetadata-schema.json
slug: amazon-app-mesh-grpcroutemetadata
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GrpcRouteMetadata\",\n  \"description\": \"An object that represents the match metadata for the route.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invert\": {},\n    \"match\": {},\n    \"name\": {}\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-grpcroutemetadata-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: GrpcRouteMetadata
---
