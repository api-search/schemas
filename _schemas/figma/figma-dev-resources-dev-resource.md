---
description: A dev resource in a file
layout: schema
name: DevResource
properties_list:
- description: Unique identifier of the dev resource
  name: id
  type: string
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
schema_file: json-schema/figma-dev-resources-dev-resource-schema.json
slug: figma-dev-resources-dev-resource
source_filename: figma-dev-resources-dev-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DevResource\",\n  \"type\": \"object\",\n  \"description\": \"A dev resource in a file\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the dev resource\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dev resource.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the dev resource.\"\n    },\n    \"fileKey\": {\n      \"type\": \"string\",\n      \"description\": \"The file key where the dev resource belongs.\"\n    },\n    \"nodeId\": {\n      \"type\": \"string\",\n      \"description\": \"The target node to attach the dev resource to.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-dev-resources-dev-resource-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: DevResource
---
