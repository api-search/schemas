---
description: ''
layout: schema
name: CreateDevResourceItem
properties_list:
- description: The name of the dev resource.
  name: name
  type: string
- description: The URL of the dev resource.
  name: url
  type: string
- description: The file key where the dev resource belongs.
  name: fileKey
  type: string
- description: The target node to attach the dev resource to.
  name: nodeId
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-dev-resources-create-dev-resource-item-schema.json
slug: figma-dev-resources-create-dev-resource-item
source_filename: figma-dev-resources-create-dev-resource-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateDevResourceItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dev resource.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the dev resource.\"\n    },\n    \"fileKey\": {\n      \"type\": \"string\",\n      \"description\": \"The file key where the dev resource belongs.\"\n    },\n    \"nodeId\": {\n      \"type\": \"string\",\n      \"description\": \"The target node to attach the dev resource to.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-dev-resources-create-dev-resource-item-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: CreateDevResourceItem
---
