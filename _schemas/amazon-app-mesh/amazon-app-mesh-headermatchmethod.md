---
description: An object that represents the method and value to match with the header value sent in a request. Specify one match method.
layout: schema
name: HeaderMatchMethod
properties_list:
- description: ''
  name: exact
  type: object
- description: ''
  name: prefix
  type: object
- description: ''
  name: range
  type: object
- description: ''
  name: regex
  type: object
- description: ''
  name: suffix
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-headermatchmethod-schema.json
slug: amazon-app-mesh-headermatchmethod
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HeaderMatchMethod\",\n  \"description\": \"An object that represents the method and value to match with the header value sent in a request. Specify one match method.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exact\": {},\n    \"prefix\": {},\n    \"range\": {},\n    \"regex\": {},\n    \"suffix\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-headermatchmethod-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: HeaderMatchMethod
---
