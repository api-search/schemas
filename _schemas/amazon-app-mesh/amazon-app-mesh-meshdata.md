---
description: An object that represents a service mesh returned by a describe operation.
layout: schema
name: MeshData
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
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-meshdata-schema.json
slug: amazon-app-mesh-meshdata
source_filename: amazon-app-mesh-meshdata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MeshData\",\n  \"description\": \"An object that represents a service mesh returned by a describe operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meshName\": {},\n    \"metadata\": {},\n    \"spec\": {},\n    \"status\": {}\n  },\n  \"required\": [\n    \"meshName\",\n    \"metadata\",\n    \"spec\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-meshdata-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: MeshData
---
