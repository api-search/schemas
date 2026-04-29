---
description: ''
layout: schema
name: LogEvent
properties_list:
- description: Unique event identifier
  name: id
  type: string
- description: Event timestamp in milliseconds
  name: timestamp
  type: integer
- description: Raw log message
  name: logmsg
  type: string
- description: Detected log types
  name: logtypes
  type: array
- description: Parsed event fields
  name: event
  type: object
- description: Tags associated with the event
  name: tags
  type: array
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-loggly-log-event-schema.json
slug: solarwinds-loggly-log-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogEvent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique event identifier\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Event timestamp in milliseconds\"\n    },\n    \"logmsg\": {\n      \"type\": \"string\",\n      \"description\": \"Raw log message\"\n    },\n    \"logtypes\": {\n      \"type\": \"array\",\n      \"description\": \"Detected log types\"\n    },\n    \"event\": {\n      \"type\": \"object\",\n      \"description\": \"Parsed event fields\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the event\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-loggly-log-event-schema.json
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
title: LogEvent
---
