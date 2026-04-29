---
description: An object that represents a virtual service backend for a virtual node.
layout: schema
name: VirtualServiceBackend
properties_list:
- description: ''
  name: clientPolicy
  type: object
- description: ''
  name: virtualServiceName
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualservicebackend-schema.json
slug: amazon-app-mesh-virtualservicebackend
source_filename: amazon-app-mesh-virtualservicebackend-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualServiceBackend\",\n  \"description\": \"An object that represents a virtual service backend for a virtual node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientPolicy\": {},\n    \"virtualServiceName\": {}\n  },\n  \"required\": [\n    \"virtualServiceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualservicebackend-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: VirtualServiceBackend
---
