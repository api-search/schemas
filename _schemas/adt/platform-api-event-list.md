---
description: Paginated list of security events.
layout: schema
name: EventList
properties_list:
- description: Array of security events.
  name: events
  type: array
- description: Total number of events matching the query.
  name: total
  type: integer
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-event-list-schema.json
slug: platform-api-event-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-event-list-schema.json\",\n  \"title\": \"EventList\",\n  \"description\": \"Paginated list of security events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Array of security events.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A security event or alarm history entry.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier of the event.\",\n            \"example\": \"evt-001\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Type of security event.\",\n            \"enum\": [\n              \"alarm\",\n              \"arm\",\n              \"disarm\",\n   \
  \           \"sensor_open\",\n              \"sensor_close\",\n              \"motion\",\n              \"video\",\n              \"panic\"\n            ],\n            \"example\": \"alarm\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable description of the event.\",\n            \"example\": \"Motion detected at front door\"\n          },\n          \"deviceId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the device that triggered the event.\",\n            \"example\": \"dev-001\"\n          },\n          \"timestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp when the event occurred.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"userId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the user associated with the event.\",\n          \
  \  \"example\": \"usr-001\"\n          }\n        }\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of events matching the query.\",\n      \"example\": 150\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-event-list-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: EventList
---
