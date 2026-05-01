---
description: An object that represents an HTTP gateway route.
layout: schema
name: HttpGatewayRoute
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: match
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-httpgatewayroute-schema.json
slug: amazon-app-mesh-httpgatewayroute
source_filename: amazon-app-mesh-httpgatewayroute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HttpGatewayRoute\",\n  \"description\": \"An object that represents an HTTP gateway route.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {},\n    \"match\": {}\n  },\n  \"required\": [\n    \"action\",\n    \"match\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-httpgatewayroute-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: HttpGatewayRoute
---
