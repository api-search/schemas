---
description: ''
layout: schema
name: Check
properties_list:
- description: Unique check identifier
  name: id
  type: integer
- description: Check name
  name: name
  type: string
- description: Check type
  name: type
  type: string
- description: Target hostname
  name: hostname
  type: string
- description: Current check status
  name: status
  type: string
- description: Check interval in minutes
  name: resolution
  type: integer
- description: Last response time in milliseconds
  name: lastresponsetime
  type: integer
- description: Last test timestamp (Unix)
  name: lasttesttime
  type: integer
- description: Creation timestamp (Unix)
  name: created
  type: integer
- description: ''
  name: tags
  type: array
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-pingdom-check-schema.json
slug: solarwinds-pingdom-check
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Check\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique check identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Check name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Check type\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Target hostname\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current check status\"\n    },\n    \"resolution\": {\n      \"type\": \"integer\",\n      \"description\": \"Check interval in minutes\"\n    },\n    \"lastresponsetime\": {\n      \"type\": \"integer\",\n      \"description\": \"Last response time in milliseconds\"\n    },\n    \"lasttesttime\": {\n      \"type\": \"integer\",\n      \"description\": \"Last test timestamp (Unix)\"\
  \n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation timestamp (Unix)\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-pingdom-check-schema.json
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
title: Check
---
