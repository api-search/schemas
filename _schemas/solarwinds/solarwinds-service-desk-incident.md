---
description: ''
layout: schema
name: Incident
properties_list:
- description: Unique incident identifier
  name: id
  type: integer
- description: Human-readable incident number
  name: number
  type: integer
- description: Incident title
  name: name
  type: string
- description: Incident description
  name: description
  type: string
- description: Current state
  name: state
  type: string
- description: Priority level
  name: priority
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-service-desk-incident-schema.json
slug: solarwinds-service-desk-incident
source_filename: solarwinds-service-desk-incident-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Incident\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique incident identifier\"\n    },\n    \"number\": {\n      \"type\": \"integer\",\n      \"description\": \"Human-readable incident number\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Incident title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Incident description\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Priority level\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-service-desk-incident-schema.json
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
title: Incident
---
