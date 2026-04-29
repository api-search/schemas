---
description: An object that represents the requirements for a route to match HTTP requests for a virtual router.
layout: schema
name: HttpRouteMatch
properties_list:
- description: ''
  name: headers
  type: object
- description: ''
  name: method
  type: object
- description: ''
  name: path
  type: object
- description: ''
  name: port
  type: object
- description: ''
  name: prefix
  type: object
- description: ''
  name: queryParameters
  type: object
- description: ''
  name: scheme
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-httproutematch-schema.json
slug: amazon-app-mesh-httproutematch
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HttpRouteMatch\",\n  \"description\": \"An object that represents the requirements for a route to match HTTP requests for a virtual router.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"headers\": {},\n    \"method\": {},\n    \"path\": {},\n    \"port\": {},\n    \"prefix\": {},\n    \"queryParameters\": {},\n    \"scheme\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-httproutematch-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: HttpRouteMatch
---
