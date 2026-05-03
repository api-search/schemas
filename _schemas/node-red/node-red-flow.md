---
description: Schema for a Node-RED flow exported via the Admin API.
layout: schema
name: Node-RED Flow
properties_list:
- description: Unique identifier for the flow node
  name: id
  type: string
- description: Node type (tab, inject, function, etc.)
  name: type
  type: string
- description: Human-readable label for the flow tab
  name: label
  type: string
- description: Node name within the flow
  name: name
  type: string
- description: Whether the flow is disabled
  name: disabled
  type: boolean
- description: Description / documentation for the flow
  name: info
  type: string
- description: Environment variables scoped to the flow
  name: env
  type: array
- description: Output wiring connections to other nodes
  name: wires
  type: array
- description: Identifier of the parent tab
  name: z
  type: string
- description: ''
  name: x
  type: number
- description: ''
  name: y
  type: number
provider_name: Node-RED
provider_slug: node-red
schema_file: json-schema/node-red-flow-schema.json
slug: node-red-flow
source_filename: node-red-flow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/json-schema/node-red-flow-schema.json\",\n  \"title\": \"Node-RED Flow\",\n  \"description\": \"Schema for a Node-RED flow exported via the Admin API.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier for the flow node\" },\n    \"type\": { \"type\": \"string\", \"description\": \"Node type (tab, inject, function, etc.)\" },\n    \"label\": { \"type\": \"string\", \"description\": \"Human-readable label for the flow tab\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Node name within the flow\" },\n    \"disabled\": { \"type\": \"boolean\", \"description\": \"Whether the flow is disabled\" },\n    \"info\": { \"type\": \"string\", \"description\": \"Description / documentation for the flow\" },\n \
  \   \"env\": {\n      \"type\": \"array\",\n      \"description\": \"Environment variables scoped to the flow\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"value\": { \"type\": \"string\" },\n          \"type\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"wires\": {\n      \"type\": \"array\",\n      \"description\": \"Output wiring connections to other nodes\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": { \"type\": \"string\" }\n      }\n    },\n    \"z\": { \"type\": \"string\", \"description\": \"Identifier of the parent tab\" },\n    \"x\": { \"type\": \"number\" },\n    \"y\": { \"type\": \"number\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/json-schema/node-red-flow-schema.json
tags:
- Self-Hosted
- Workflow Automation
- Flow-Based Programming
- IoT
title: Node-RED Flow
---
