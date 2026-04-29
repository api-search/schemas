---
description: ApplicationScore schema from Palo Alto Networks Autonomous DEM API
layout: schema
name: ApplicationScore
properties_list:
- description: Time bucket for the aggregated score.
  name: timestamp
  type: string
- description: Monitored application identifier.
  name: app_id
  type: string
- description: Name of the monitored application.
  name: application
  type: string
- description: User identifier if filtering by user.
  name: user_id
  type: string
- description: Site name if filtering by site.
  name: site_name
  type: string
- description: Overall experience score from 0 to 100.
  name: overall_score
  type: integer
- description: Endpoint health score.
  name: endpoint_score
  type: integer
- description: Network path score.
  name: network_score
  type: integer
- description: Application responsiveness score.
  name: application_score
  type: integer
- description: Average round-trip latency in milliseconds.
  name: latency_ms
  type: number
- description: Packet loss percentage.
  name: packet_loss_pct
  type: number
- description: Latency variation in milliseconds.
  name: jitter_ms
  type: number
- description: Number of measurement samples in this time bucket.
  name: sample_count
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/autonomous-dem-api-application-score-schema.json
slug: autonomous-dem-api-application-score
source_filename: autonomous-dem-api-application-score-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationScore\",\n  \"description\": \"ApplicationScore schema from Palo Alto Networks Autonomous DEM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-application-score-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time bucket for the aggregated score.\"\n    },\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"Monitored application identifier.\"\n    },\n    \"application\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the monitored application.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"User identifier if filtering by user.\"\n    },\n    \"site_name\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Site name if filtering by site.\"\n    },\n    \"overall_score\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Overall experience score from 0 to 100.\"\n    },\n    \"endpoint_score\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Endpoint health score.\"\n    },\n    \"network_score\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Network path score.\"\n    },\n    \"application_score\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Application responsiveness score.\"\n    },\n    \"latency_ms\": {\n      \"type\": \"number\",\n      \"description\": \"Average round-trip latency in milliseconds.\"\n    },\n    \"packet_loss_pct\": {\n      \"type\": \"number\",\n      \"description\": \"Packet loss percentage.\"\n    },\n    \"jitter_ms\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Latency variation in milliseconds.\"\n    },\n    \"sample_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of measurement samples in this time bucket.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-application-score-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ApplicationScore
---
