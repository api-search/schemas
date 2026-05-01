---
description: <zonbook></zonbook><xhtml></xhtml>
layout: schema
name: UntagResourceInput
properties_list:
- description: ''
  name: tagKeys
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-untag-resource-input-schema.json
slug: app-mesh-untag-resource-input
source_filename: app-mesh-untag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"tagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \"The keys of the tags to be removed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"tagKeys\"\n  ],\n  \"description\": \"<zonbook></zonbook><xhtml></xhtml>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-untag-resource-input-schema.json\",\n  \"title\": \"UntagResourceInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-untag-resource-input-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: UntagResourceInput
---
