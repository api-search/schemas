---
description: Physical or virtual hardware node managed by Acronis
layout: schema
name: HardwareNode
properties_list:
- description: Hardware node identifier
  name: id
  type: string
- description: Node hostname
  name: hostname
  type: string
- description: Node type
  name: type
  type: string
- description: Node operational status
  name: status
  type: string
- description: ''
  name: tenant_id
  type: string
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/agent-management-hardware-node-schema.json
slug: agent-management-hardware-node
source_filename: agent-management-hardware-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/agent-management-hardware-node-schema.json\",\n  \"title\": \"HardwareNode\",\n  \"description\": \"Physical or virtual hardware node managed by Acronis\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware node identifier\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Node hostname\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Node type\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Node operational status\"\n    },\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/agent-management-hardware-node-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: HardwareNode
---
