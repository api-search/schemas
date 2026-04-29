---
description: AgentScore schema from Palo Alto Networks Autonomous DEM API
layout: schema
name: AgentScore
properties_list:
- description: Time bucket for the aggregated score.
  name: timestamp
  type: string
- description: Unique ADEM agent identifier.
  name: agent_id
  type: string
- description: User identifier associated with the agent.
  name: user_id
  type: string
- description: Hostname of the endpoint device.
  name: device_name
  type: string
- description: Site name where the agent is located.
  name: site_name
  type: string
- description: Overall experience score for this agent.
  name: overall_score
  type: integer
- description: Endpoint hardware and software health score.
  name: endpoint_score
  type: integer
- description: Network connectivity quality score.
  name: network_score
  type: integer
- description: CPU usage percentage on the endpoint.
  name: cpu_usage_pct
  type: number
- description: Memory usage percentage on the endpoint.
  name: memory_usage_pct
  type: number
- description: Number of measurement samples in this time bucket.
  name: sample_count
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/autonomous-dem-api-agent-score-schema.json
slug: autonomous-dem-api-agent-score
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgentScore\",\n  \"description\": \"AgentScore schema from Palo Alto Networks Autonomous DEM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-agent-score-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time bucket for the aggregated score.\"\n    },\n    \"agent_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ADEM agent identifier.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"User identifier associated with the agent.\"\n    },\n    \"device_name\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the endpoint device.\"\n    },\n    \"site_name\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Site name where the agent is located.\"\n    },\n    \"overall_score\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Overall experience score for this agent.\"\n    },\n    \"endpoint_score\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Endpoint hardware and software health score.\"\n    },\n    \"network_score\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Network connectivity quality score.\"\n    },\n    \"cpu_usage_pct\": {\n      \"type\": \"number\",\n      \"description\": \"CPU usage percentage on the endpoint.\"\n    },\n    \"memory_usage_pct\": {\n      \"type\": \"number\",\n      \"description\": \"Memory usage percentage on the endpoint.\"\n    },\n    \"sample_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of measurement samples in this time bucket.\"\n    }\n  }\n\
  }\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-agent-score-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AgentScore
---
