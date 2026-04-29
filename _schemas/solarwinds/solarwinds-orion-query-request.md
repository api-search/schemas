---
description: ''
layout: schema
name: QueryRequest
properties_list:
- description: SWQL query string to execute
  name: query
  type: string
- description: Named parameters for parameterized queries
  name: parameters
  type: object
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-orion-query-request-schema.json
slug: solarwinds-orion-query-request
source_filename: solarwinds-orion-query-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"SWQL query string to execute\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Named parameters for parameterized queries\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-orion-query-request-schema.json
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
title: QueryRequest
---
