---
description: An object that represents the action to take if a match is determined.
layout: schema
name: TcpRouteAction
properties_list:
- description: ''
  name: weightedTargets
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-tcprouteaction-schema.json
slug: amazon-app-mesh-tcprouteaction
source_filename: amazon-app-mesh-tcprouteaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TcpRouteAction\",\n  \"description\": \"An object that represents the action to take if a match is determined.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"weightedTargets\": {}\n  },\n  \"required\": [\n    \"weightedTargets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-tcprouteaction-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: TcpRouteAction
---
