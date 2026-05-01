---
description: ''
layout: schema
name: Dell Server
properties_list:
- description: Unique Dell service tag identifier.
  name: service_tag
  type: string
- description: Dell server model (e.g. PowerEdge R750).
  name: model
  type: string
- description: Administrator-assigned name for the server.
  name: name
  type: string
- description: Operational status of the server.
  name: status
  type: string
- description: Current firmware version installed on the server.
  name: firmware_version
  type: string
provider_name: Dell Technologies
provider_slug: dell-technologies
schema_file: json-schema/dell-server-schema.json
slug: dell-server
source_filename: dell-server-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.dell.com/server.json\",\n  \"title\": \"Dell Server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service_tag\": {\"type\": \"string\", \"description\": \"Unique Dell service tag identifier.\"},\n    \"model\": {\"type\": \"string\", \"description\": \"Dell server model (e.g. PowerEdge R750).\"},\n    \"name\": {\"type\": \"string\", \"description\": \"Administrator-assigned name for the server.\"},\n    \"status\": {\"type\": \"string\", \"description\": \"Operational status of the server.\"},\n    \"firmware_version\": {\"type\": \"string\", \"description\": \"Current firmware version installed on the server.\"}\n  },\n  \"required\": [\"service_tag\", \"model\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dell-technologies/refs/heads/main/json-schema/dell-server-schema.json
tags:
- Enterprise IT
- Infrastructure
- Servers
- Storage
- Cloud
- Automation
title: Dell Server
---
