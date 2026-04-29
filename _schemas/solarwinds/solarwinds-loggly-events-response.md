---
description: ''
layout: schema
name: EventsResponse
properties_list:
- description: Total number of matching events
  name: total_events
  type: integer
- description: Current page number
  name: page
  type: integer
- description: ''
  name: events
  type: array
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-loggly-events-response-schema.json
slug: solarwinds-loggly-events-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total_events\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching events\"\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\"\n    },\n    \"events\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-loggly-events-response-schema.json
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
title: EventsResponse
---
