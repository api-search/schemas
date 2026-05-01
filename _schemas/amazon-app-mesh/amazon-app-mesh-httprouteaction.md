---
description: An object that represents the action to take if a match is determined.
layout: schema
name: HttpRouteAction
properties_list:
- description: ''
  name: weightedTargets
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-httprouteaction-schema.json
slug: amazon-app-mesh-httprouteaction
source_filename: amazon-app-mesh-httprouteaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HttpRouteAction\",\n  \"description\": \"An object that represents the action to take if a match is determined.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"weightedTargets\": {}\n  },\n  \"required\": [\n    \"weightedTargets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-httprouteaction-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: HttpRouteAction
---
