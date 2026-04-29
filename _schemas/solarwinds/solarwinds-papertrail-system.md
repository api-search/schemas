---
description: ''
layout: schema
name: System
properties_list:
- description: System ID
  name: id
  type: integer
- description: System name
  name: name
  type: string
- description: ''
  name: last_event_at
  type: string
- description: ''
  name: auto_delete
  type: boolean
- description: ''
  name: ip_address
  type: string
- description: ''
  name: hostname
  type: string
- description: ''
  name: syslog
  type: object
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-papertrail-system-schema.json
slug: solarwinds-papertrail-system
source_filename: solarwinds-papertrail-system-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"System\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"System ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"System name\"\n    },\n    \"last_event_at\": {\n      \"type\": \"string\"\n    },\n    \"auto_delete\": {\n      \"type\": \"boolean\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\"\n    },\n    \"hostname\": {\n      \"type\": \"string\"\n    },\n    \"syslog\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-papertrail-system-schema.json
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
title: System
---
