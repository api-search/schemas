---
description: ''
layout: schema
name: Event
properties_list:
- description: Unique event identifier
  name: id
  type: string
- description: When the event was received
  name: received_at
  type: string
- description: When the event was generated
  name: generated_at
  type: string
- description: Human-readable received timestamp
  name: display_received_at
  type: string
- description: Source IP address
  name: source_ip
  type: string
- description: Source system name
  name: source_name
  type: string
- description: Source system ID
  name: source_id
  type: integer
- description: Hostname
  name: hostname
  type: string
- description: Program name
  name: program
  type: string
- description: Syslog severity
  name: severity
  type: string
- description: Syslog facility
  name: facility
  type: string
- description: Log message content
  name: message
  type: string
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-papertrail-event-schema.json
slug: solarwinds-papertrail-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique event identifier\"\n    },\n    \"received_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the event was received\"\n    },\n    \"generated_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the event was generated\"\n    },\n    \"display_received_at\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable received timestamp\"\n    },\n    \"source_ip\": {\n      \"type\": \"string\",\n      \"description\": \"Source IP address\"\n    },\n    \"source_name\": {\n      \"type\": \"string\",\n      \"description\": \"Source system name\"\n    },\n    \"source_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Source system ID\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Hostname\"\n    },\n    \"program\": {\n      \"type\": \"string\",\n      \"description\": \"Program name\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Syslog severity\"\n    },\n    \"facility\": {\n      \"type\": \"string\",\n      \"description\": \"Syslog facility\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Log message content\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-papertrail-event-schema.json
tags:
- Application Monitoring
- Database Monitoring
- Infrastructure
- IP Address Management
- IT Management
- ITSM
- Log Management
- Network Monitoring
- Observability
title: Event
---
