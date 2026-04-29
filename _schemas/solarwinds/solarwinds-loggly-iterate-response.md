---
description: ''
layout: schema
name: IterateResponse
properties_list:
- description: ''
  name: events
  type: array
- description: Cursor for next page of results
  name: next
  type: string
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-loggly-iterate-response-schema.json
slug: solarwinds-loggly-iterate-response
source_filename: solarwinds-loggly-iterate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IterateResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"events\": {\n      \"type\": \"array\"\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-loggly-iterate-response-schema.json
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
title: IterateResponse
---
