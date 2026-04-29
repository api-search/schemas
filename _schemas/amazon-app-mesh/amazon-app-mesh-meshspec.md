---
description: An object that represents the specification of a service mesh.
layout: schema
name: MeshSpec
properties_list:
- description: ''
  name: egressFilter
  type: object
- description: ''
  name: serviceDiscovery
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-meshspec-schema.json
slug: amazon-app-mesh-meshspec
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MeshSpec\",\n  \"description\": \"An object that represents the specification of a service mesh.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"egressFilter\": {},\n    \"serviceDiscovery\": {\n      \"$ref\": \"#/definitions/MeshServiceDiscovery\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-meshspec-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: MeshSpec
---
