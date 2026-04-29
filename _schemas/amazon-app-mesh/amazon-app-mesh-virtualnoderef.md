---
description: An object that represents a virtual node returned by a list operation.
layout: schema
name: VirtualNodeRef
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: meshName
  type: object
- description: ''
  name: meshOwner
  type: object
- description: ''
  name: resourceOwner
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: virtualNodeName
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualnoderef-schema.json
slug: amazon-app-mesh-virtualnoderef
source_filename: amazon-app-mesh-virtualnoderef-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualNodeRef\",\n  \"description\": \"An object that represents a virtual node returned by a list operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {},\n    \"createdAt\": {},\n    \"lastUpdatedAt\": {},\n    \"meshName\": {},\n    \"meshOwner\": {},\n    \"resourceOwner\": {},\n    \"version\": {},\n    \"virtualNodeName\": {}\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"lastUpdatedAt\",\n    \"meshName\",\n    \"meshOwner\",\n    \"resourceOwner\",\n    \"version\",\n    \"virtualNodeName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualnoderef-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: VirtualNodeRef
---
