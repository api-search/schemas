---
description: An object that represents a virtual router listener.
layout: schema
name: VirtualRouterListener
properties_list:
- description: ''
  name: portMapping
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualrouterlistener-schema.json
slug: amazon-app-mesh-virtualrouterlistener
source_filename: amazon-app-mesh-virtualrouterlistener-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualRouterListener\",\n  \"description\": \"An object that represents a virtual router listener.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portMapping\": {\n      \"$ref\": \"#/definitions/PortMapping\"\n    }\n  },\n  \"required\": [\n    \"portMapping\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualrouterlistener-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: VirtualRouterListener
---
