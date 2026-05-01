---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: UpdateVirtualNodeInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: spec
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-update-virtual-node-input-schema.json
slug: app-mesh-update-virtual-node-input
source_filename: app-mesh-update-virtual-node-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request. Up to 36 letters, numbers, hyphens, and underscores are allowed.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualNodeSpec\"\n        },\n        {\n          \"description\": \"The new virtual node specification to apply. This overwrites the existing data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"spec\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-update-virtual-node-input-schema.json\"\
  ,\n  \"title\": \"UpdateVirtualNodeInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-update-virtual-node-input-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: UpdateVirtualNodeInput
---
