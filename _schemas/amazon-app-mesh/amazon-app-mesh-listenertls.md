---
description: An object that represents the Transport Layer Security (TLS) properties for a listener.
layout: schema
name: ListenerTls
properties_list:
- description: ''
  name: certificate
  type: object
- description: ''
  name: mode
  type: object
- description: ''
  name: validation
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-listenertls-schema.json
slug: amazon-app-mesh-listenertls
source_filename: amazon-app-mesh-listenertls-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ListenerTls\",\n  \"description\": \"An object that represents the Transport Layer Security (TLS) properties for a listener.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificate\": {},\n    \"mode\": {},\n    \"validation\": {}\n  },\n  \"required\": [\n    \"certificate\",\n    \"mode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-listenertls-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: ListenerTls
---
