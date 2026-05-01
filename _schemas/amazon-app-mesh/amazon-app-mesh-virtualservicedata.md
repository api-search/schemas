---
description: An object that represents a virtual service returned by a describe operation.
layout: schema
name: VirtualServiceData
properties_list:
- description: ''
  name: meshName
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: virtualServiceName
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualservicedata-schema.json
slug: amazon-app-mesh-virtualservicedata
source_filename: amazon-app-mesh-virtualservicedata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualServiceData\",\n  \"description\": \"An object that represents a virtual service returned by a describe operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meshName\": {},\n    \"metadata\": {\n      \"$ref\": \"#/definitions/ResourceMetadata\"\n    },\n    \"spec\": {},\n    \"status\": {},\n    \"virtualServiceName\": {}\n  },\n  \"required\": [\n    \"meshName\",\n    \"metadata\",\n    \"spec\",\n    \"status\",\n    \"virtualServiceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualservicedata-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: VirtualServiceData
---
