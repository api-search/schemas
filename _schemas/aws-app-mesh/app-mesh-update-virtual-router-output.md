---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: UpdateVirtualRouterOutput
properties_list:
- description: ''
  name: virtualRouter
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-update-virtual-router-output-schema.json
slug: app-mesh-update-virtual-router-output
source_filename: app-mesh-update-virtual-router-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualRouter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualRouterData\"\n        },\n        {\n          \"description\": \"A full description of the virtual router that was updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualRouter\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-update-virtual-router-output-schema.json\",\n  \"title\": \"UpdateVirtualRouterOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-update-virtual-router-output-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: UpdateVirtualRouterOutput
---
