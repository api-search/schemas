---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: DeleteVirtualServiceOutput
properties_list:
- description: ''
  name: virtualService
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-delete-virtual-service-output-schema.json
slug: app-mesh-delete-virtual-service-output
source_filename: app-mesh-delete-virtual-service-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualService\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualServiceData\"\n        },\n        {\n          \"description\": \"The virtual service that was deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualService\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-delete-virtual-service-output-schema.json\",\n  \"title\": \"DeleteVirtualServiceOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-delete-virtual-service-output-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: DeleteVirtualServiceOutput
---
