---
description: Response from the Get File Nodes endpoint.
layout: schema
name: GetFileNodesResponse
properties_list:
- description: The name of the file.
  name: name
  type: string
- description: ''
  name: lastModified
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: role
  type: string
- description: A mapping from node IDs to node data. Each value contains a document subtree and optionally the component metadata for that node.
  name: nodes
  type: object
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-get-file-nodes-response-schema.json
slug: figma-rest-get-file-nodes-response
source_filename: figma-rest-get-file-nodes-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetFileNodesResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from the Get File Nodes endpoint.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"role\": {\n      \"type\": \"string\"\n    },\n    \"nodes\": {\n      \"type\": \"object\",\n      \"description\": \"A mapping from node IDs to node data. Each value contains a document subtree and optionally the component metadata for that node.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-get-file-nodes-response-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetFileNodesResponse
---
