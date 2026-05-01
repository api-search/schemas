---
description: An object that represents the HTTP header in the request.
layout: schema
name: HttpRouteHeader
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
schema_file: json-schema/amazon-app-mesh-httprouteheader-schema.json
slug: amazon-app-mesh-httprouteheader
source_filename: amazon-app-mesh-httprouteheader-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HttpRouteHeader\",\n  \"description\": \"An object that represents the HTTP header in the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invert\": {},\n    \"match\": {},\n    \"name\": {}\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-httprouteheader-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: HttpRouteHeader
---
