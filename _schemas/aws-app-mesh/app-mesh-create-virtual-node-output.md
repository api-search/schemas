---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: CreateVirtualNodeOutput
properties_list:
- description: ''
  name: virtualNode
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-create-virtual-node-output-schema.json
slug: app-mesh-create-virtual-node-output
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualNode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualNodeData\"\n        },\n        {\n          \"description\": \"The full description of your virtual node following the create call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualNode\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-create-virtual-node-output-schema.json\",\n  \"title\": \"CreateVirtualNodeOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-create-virtual-node-output-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: CreateVirtualNodeOutput
---
