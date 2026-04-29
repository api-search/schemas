---
description: An object that represents a port mapping.
layout: schema
name: PortMapping
properties_list:
- description: ''
  name: port
  type: object
- description: ''
  name: protocol
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-portmapping-schema.json
slug: amazon-app-mesh-portmapping
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"PortMapping\",\n  \"description\": \"An object that represents a port mapping.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"port\": {},\n    \"protocol\": {}\n  },\n  \"required\": [\n    \"port\",\n    \"protocol\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-portmapping-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: PortMapping
---
