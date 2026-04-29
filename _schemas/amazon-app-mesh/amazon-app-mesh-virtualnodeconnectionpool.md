---
description: <p>An object that represents the type of virtual node connection pool.</p> <p>Only one protocol is used at a time and should be the same protocol as the one chosen under port mapping.</p> <p>If not present the default value for <code>maxPendingRequests</code> is <code>2147483647</code>.</p> <p/>
layout: schema
name: VirtualNodeConnectionPool
properties_list:
- description: ''
  name: grpc
  type: object
- description: ''
  name: http
  type: object
- description: ''
  name: http2
  type: object
- description: ''
  name: tcp
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualnodeconnectionpool-schema.json
slug: amazon-app-mesh-virtualnodeconnectionpool
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualNodeConnectionPool\",\n  \"description\": \"<p>An object that represents the type of virtual node connection pool.</p> <p>Only one protocol is used at a time and should be the same protocol as the one chosen under port mapping.</p> <p>If not present the default value for <code>maxPendingRequests</code> is <code>2147483647</code>.</p> <p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grpc\": {},\n    \"http\": {},\n    \"http2\": {},\n    \"tcp\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualnodeconnectionpool-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: VirtualNodeConnectionPool
---
