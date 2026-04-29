---
description: ''
layout: schema
name: EventSearchResult
properties_list:
- description: ''
  name: events
  type: array
- description: Minimum event ID in results
  name: min_id
  type: string
- description: Maximum event ID in results
  name: max_id
  type: string
- description: Whether results include the earliest matching event
  name: reached_beginning
  type: boolean
- description: ''
  name: min_time_at
  type: string
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-papertrail-event-search-result-schema.json
slug: solarwinds-papertrail-event-search-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventSearchResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"events\": {\n      \"type\": \"array\"\n    },\n    \"min_id\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum event ID in results\"\n    },\n    \"max_id\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum event ID in results\"\n    },\n    \"reached_beginning\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether results include the earliest matching event\"\n    },\n    \"min_time_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-papertrail-event-search-result-schema.json
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
title: EventSearchResult
---
