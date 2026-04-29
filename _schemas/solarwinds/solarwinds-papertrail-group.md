---
description: ''
layout: schema
name: Group
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: system_wildcard
  type: string
- description: ''
  name: systems
  type: array
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-papertrail-group-schema.json
slug: solarwinds-papertrail-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"system_wildcard\": {\n      \"type\": \"string\"\n    },\n    \"systems\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-papertrail-group-schema.json
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
title: Group
---
