---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: CreateVirtualServiceInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: virtualServiceName
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-createvirtualserviceinput-schema.json
slug: amazon-app-mesh-createvirtualserviceinput
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateVirtualServiceInput\",\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {},\n    \"spec\": {},\n    \"tags\": {},\n    \"virtualServiceName\": {}\n  },\n  \"required\": [\n    \"spec\",\n    \"virtualServiceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-createvirtualserviceinput-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: CreateVirtualServiceInput
---
