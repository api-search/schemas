---
description: ''
layout: schema
name: QueryResult
properties_list:
- description: Array of result rows
  name: results
  type: array
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-orion-query-result-schema.json
slug: solarwinds-orion-query-result
source_filename: solarwinds-orion-query-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of result rows\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-orion-query-result-schema.json
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
title: QueryResult
---
