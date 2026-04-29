---
description: Acronis protection agent registered on an endpoint
layout: schema
name: Agent
properties_list:
- description: Agent unique identifier
  name: id
  type: string
- description: Hostname of the protected machine
  name: hostname
  type: string
- description: Current agent connection status
  name: status
  type: string
- description: Agent software version
  name: version
  type: string
- description: Tenant this agent belongs to
  name: tenant_id
  type: string
- description: ''
  name: os
  type: object
- description: Last time agent communicated with the platform
  name: last_seen
  type: string
- description: ''
  name: registration_time
  type: string
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/agent-management-agent-schema.json
slug: agent-management-agent
source_filename: agent-management-agent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/agent-management-agent-schema.json\",\n  \"title\": \"Agent\",\n  \"description\": \"Acronis protection agent registered on an endpoint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Agent unique identifier\",\n      \"example\": \"agent-uuid-001\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the protected machine\",\n      \"example\": \"workstation-01\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"online\",\n        \"offline\",\n        \"unknown\"\n      ],\n      \"description\": \"Current agent connection status\",\n      \"example\": \"online\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Agent software version\"\
  ,\n      \"example\": \"21.12.30\"\n    },\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Tenant this agent belongs to\"\n    },\n    \"os\": {\n      \"$ref\": \"#/components/schemas/AgentOS\"\n    },\n    \"last_seen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last time agent communicated with the platform\"\n    },\n    \"registration_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/agent-management-agent-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: Agent
---
