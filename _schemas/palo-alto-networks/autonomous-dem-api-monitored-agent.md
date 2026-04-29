---
description: MonitoredAgent schema from Palo Alto Networks Autonomous DEM API
layout: schema
name: MonitoredAgent
properties_list:
- description: Unique ADEM agent identifier.
  name: agent_id
  type: string
- description: User email or identifier associated with this agent.
  name: user_id
  type: string
- description: Hostname of the endpoint device.
  name: device_name
  type: string
- description: Operating system of the endpoint.
  name: os
  type: string
- description: Operating system version string.
  name: os_version
  type: string
- description: ADEM agent software version.
  name: agent_version
  type: string
- description: Site name where the agent is located.
  name: site_name
  type: string
- description: Current agent connectivity status.
  name: status
  type: string
- description: Timestamp of the last agent heartbeat.
  name: last_seen
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/autonomous-dem-api-monitored-agent-schema.json
slug: autonomous-dem-api-monitored-agent
source_filename: autonomous-dem-api-monitored-agent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MonitoredAgent\",\n  \"description\": \"MonitoredAgent schema from Palo Alto Networks Autonomous DEM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-monitored-agent-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agent_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ADEM agent identifier.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"User email or identifier associated with this agent.\"\n    },\n    \"device_name\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the endpoint device.\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"windows\",\n        \"macos\",\n        \"linux\",\n        \"ios\",\n        \"android\"\n      ],\n      \"description\": \"Operating system\
  \ of the endpoint.\"\n    },\n    \"os_version\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system version string.\"\n    },\n    \"agent_version\": {\n      \"type\": \"string\",\n      \"description\": \"ADEM agent software version.\"\n    },\n    \"site_name\": {\n      \"type\": \"string\",\n      \"description\": \"Site name where the agent is located.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"connected\",\n        \"disconnected\",\n        \"degraded\"\n      ],\n      \"description\": \"Current agent connectivity status.\"\n    },\n    \"last_seen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last agent heartbeat.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-monitored-agent-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MonitoredAgent
---
