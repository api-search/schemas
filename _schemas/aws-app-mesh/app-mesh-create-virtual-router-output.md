---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: CreateVirtualRouterOutput
properties_list:
- description: ''
  name: virtualRouter
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-create-virtual-router-output-schema.json
slug: app-mesh-create-virtual-router-output
source_filename: app-mesh-create-virtual-router-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualRouter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualRouterData\"\n        },\n        {\n          \"description\": \"The full description of your virtual router following the create call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualRouter\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-create-virtual-router-output-schema.json\",\n  \"title\": \"CreateVirtualRouterOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-create-virtual-router-output-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: CreateVirtualRouterOutput
---
