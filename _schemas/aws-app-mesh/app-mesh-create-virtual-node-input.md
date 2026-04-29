---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: CreateVirtualNodeInput
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
  name: virtualNodeName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-create-virtual-node-input-schema.json
slug: app-mesh-create-virtual-node-input
source_filename: app-mesh-create-virtual-node-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request. Up to 36 letters, numbers, hyphens, and underscores are allowed.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualNodeSpec\"\n        },\n        {\n          \"description\": \"The virtual node specification to apply.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Optional metadata that you can apply to the virtual node to assist with categorization and organization. Each tag consists of a key and an optional value, both of which you define. Tag keys can have a maximum\
  \ character length of 128 characters, and tag values can have a maximum length of 256 characters.\"\n        }\n      ]\n    },\n    \"virtualNodeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name to use for the virtual node.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"spec\",\n    \"virtualNodeName\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-create-virtual-node-input-schema.json\",\n  \"title\": \"CreateVirtualNodeInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-create-virtual-node-input-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: CreateVirtualNodeInput
---
