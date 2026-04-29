---
description: An object that represents types of timeouts.
layout: schema
name: GrpcTimeout
properties_list:
- description: ''
  name: idle
  type: object
- description: ''
  name: perRequest
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-grpctimeout-schema.json
slug: amazon-app-mesh-grpctimeout
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GrpcTimeout\",\n  \"description\": \"An object that represents types of timeouts. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"idle\": {},\n    \"perRequest\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-grpctimeout-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: GrpcTimeout
---
