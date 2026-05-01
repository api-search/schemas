---
description: An object that represents the specification of a virtual node.
layout: schema
name: VirtualNodeSpec
properties_list:
- description: ''
  name: backendDefaults
  type: object
- description: ''
  name: backends
  type: object
- description: ''
  name: listeners
  type: object
- description: ''
  name: logging
  type: object
- description: ''
  name: serviceDiscovery
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualnodespec-schema.json
slug: amazon-app-mesh-virtualnodespec
source_filename: amazon-app-mesh-virtualnodespec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualNodeSpec\",\n  \"description\": \"An object that represents the specification of a virtual node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"backendDefaults\": {},\n    \"backends\": {},\n    \"listeners\": {},\n    \"logging\": {},\n    \"serviceDiscovery\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualnodespec-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: VirtualNodeSpec
---
