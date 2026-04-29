---
description: An object that represents a type of connection pool.
layout: schema
name: VirtualNodeHttpConnectionPool
properties_list:
- description: ''
  name: maxConnections
  type: object
- description: ''
  name: maxPendingRequests
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualnodehttpconnectionpool-schema.json
slug: amazon-app-mesh-virtualnodehttpconnectionpool
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualNodeHttpConnectionPool\",\n  \"description\": \"An object that represents a type of connection pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxConnections\": {},\n    \"maxPendingRequests\": {}\n  },\n  \"required\": [\n    \"maxConnections\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualnodehttpconnectionpool-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: VirtualNodeHttpConnectionPool
---
