---
description: An object that represents a listener for a virtual node.
layout: schema
name: Listener
properties_list:
- description: ''
  name: connectionPool
  type: object
- description: ''
  name: healthCheck
  type: object
- description: ''
  name: outlierDetection
  type: object
- description: ''
  name: portMapping
  type: object
- description: ''
  name: timeout
  type: object
- description: ''
  name: tls
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-listener-schema.json
slug: amazon-app-mesh-listener
source_filename: amazon-app-mesh-listener-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Listener\",\n  \"description\": \"An object that represents a listener for a virtual node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionPool\": {},\n    \"healthCheck\": {},\n    \"outlierDetection\": {},\n    \"portMapping\": {},\n    \"timeout\": {},\n    \"tls\": {}\n  },\n  \"required\": [\n    \"portMapping\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-listener-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: Listener
---
