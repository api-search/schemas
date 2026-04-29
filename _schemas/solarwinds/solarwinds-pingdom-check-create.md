---
description: ''
layout: schema
name: CheckCreate
properties_list:
- description: Check name
  name: name
  type: string
- description: Target hostname or IP
  name: host
  type: string
- description: Check type
  name: type
  type: string
- description: Check interval in minutes
  name: resolution
  type: integer
- description: Whether the check is paused
  name: paused
  type: boolean
- description: Use SSL/TLS
  name: encryption
  type: boolean
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-pingdom-check-create-schema.json
slug: solarwinds-pingdom-check-create
source_filename: solarwinds-pingdom-check-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CheckCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Check name\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Target hostname or IP\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Check type\"\n    },\n    \"resolution\": {\n      \"type\": \"integer\",\n      \"description\": \"Check interval in minutes\"\n    },\n    \"paused\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the check is paused\"\n    },\n    \"encryption\": {\n      \"type\": \"boolean\",\n      \"description\": \"Use SSL/TLS\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-pingdom-check-create-schema.json
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
title: CheckCreate
---
