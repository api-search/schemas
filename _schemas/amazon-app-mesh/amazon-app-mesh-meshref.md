---
description: An object that represents a service mesh returned by a list operation.
layout: schema
name: MeshRef
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
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-meshref-schema.json
slug: amazon-app-mesh-meshref
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MeshRef\",\n  \"description\": \"An object that represents a service mesh returned by a list operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {},\n    \"createdAt\": {},\n    \"lastUpdatedAt\": {},\n    \"meshName\": {},\n    \"meshOwner\": {},\n    \"resourceOwner\": {},\n    \"version\": {}\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"lastUpdatedAt\",\n    \"meshName\",\n    \"meshOwner\",\n    \"resourceOwner\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-meshref-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: MeshRef
---
