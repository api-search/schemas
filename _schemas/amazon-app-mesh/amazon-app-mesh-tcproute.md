---
description: An object that represents a TCP route type.
layout: schema
name: TcpRoute
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: match
  type: object
- description: ''
  name: timeout
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-tcproute-schema.json
slug: amazon-app-mesh-tcproute
source_filename: amazon-app-mesh-tcproute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TcpRoute\",\n  \"description\": \"An object that represents a TCP route type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {},\n    \"match\": {},\n    \"timeout\": {}\n  },\n  \"required\": [\n    \"action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-tcproute-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: TcpRoute
---
