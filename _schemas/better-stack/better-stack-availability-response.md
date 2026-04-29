---
description: Availability summary metrics.
layout: schema
name: AvailabilityResponse
properties_list:
- description: ''
  name: data
  type: object
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-availability-response-schema.json
slug: better-stack-availability-response
source_filename: better-stack-availability-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-availability-response-schema.json\",\n  \"title\": \"AvailabilityResponse\",\n  \"description\": \"Availability summary metrics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"availability\": {\n          \"type\": \"number\",\n          \"description\": \"Availability percentage.\",\n          \"example\": 99.98\n        },\n        \"downtime_duration\": {\n          \"type\": \"integer\",\n          \"description\": \"Total downtime duration in seconds.\",\n          \"example\": 86\n        },\n        \"number_of_incidents\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of incidents in the period.\",\n          \"example\": 2\n        },\n        \"longest_incident_duration\":\
  \ {\n          \"type\": \"integer\",\n          \"description\": \"Duration of the longest incident in seconds.\",\n          \"example\": 61\n        },\n        \"average_incident_duration\": {\n          \"type\": \"integer\",\n          \"description\": \"Average incident duration in seconds.\",\n          \"example\": 43\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-availability-response-schema.json
tags:
- Incidents
- Logs
- Monitoring
- Platform
- Status
- Uptime
- Observability
- On-Call
- Heartbeats
title: AvailabilityResponse
---
