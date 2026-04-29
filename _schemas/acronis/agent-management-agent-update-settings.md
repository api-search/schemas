---
description: Configuration for automatic agent updates
layout: schema
name: AgentUpdateSettings
properties_list:
- description: Update channel to use
  name: update_channel
  type: string
- description: Whether updates should be applied automatically
  name: automatic
  type: boolean
- description: ''
  name: maintenance_window
  type: object
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/agent-management-agent-update-settings-schema.json
slug: agent-management-agent-update-settings
source_filename: agent-management-agent-update-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/agent-management-agent-update-settings-schema.json\",\n  \"title\": \"AgentUpdateSettings\",\n  \"description\": \"Configuration for automatic agent updates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"update_channel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CURRENT\",\n        \"STABLE\"\n      ],\n      \"description\": \"Update channel to use\",\n      \"example\": \"STABLE\"\n    },\n    \"automatic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether updates should be applied automatically\",\n      \"example\": true\n    },\n    \"maintenance_window\": {\n      \"$ref\": \"#/components/schemas/MaintenanceWindow\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/agent-management-agent-update-settings-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: AgentUpdateSettings
---
