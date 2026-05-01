---
description: An object that represents timeouts for different protocols.
layout: schema
name: ListenerTimeout
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
schema_file: json-schema/amazon-app-mesh-listenertimeout-schema.json
slug: amazon-app-mesh-listenertimeout
source_filename: amazon-app-mesh-listenertimeout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ListenerTimeout\",\n  \"description\": \"An object that represents timeouts for different protocols.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grpc\": {},\n    \"http\": {},\n    \"http2\": {},\n    \"tcp\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-listenertimeout-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: ListenerTimeout
---
