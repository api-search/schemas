---
description: Represents a single event in the Dynatrace environment. Events can be ingested via the API or detected automatically by Dynatrace.
layout: schema
name: Event
properties_list:
- description: The unique identifier of the event.
  name: eventId
  type: string
- description: The type of the event.
  name: eventType
  type: string
- description: The display title of the event.
  name: title
  type: string
- description: The start time of the event as a Unix timestamp in milliseconds.
  name: startTime
  type: integer
- description: The end time of the event as a Unix timestamp in milliseconds. Null for open events.
  name: endTime
  type: integer
- description: ''
  name: entityId
  type: object
- description: Additional key-value metadata attached to the event.
  name: properties
  type: object
- description: The current status of the event. OPEN indicates the event is still active; CLOSED indicates it has ended.
  name: status
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/events-api-v2-event-schema.json
slug: events-api-v2-event
source_filename: events-api-v2-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/events-api-v2-event-schema.json\",\n  \"title\": \"Event\",\n  \"description\": \"Represents a single event in the Dynatrace environment. Events can be ingested via the API or detected automatically by Dynatrace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the event.\",\n      \"example\": \"abc123\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the event.\",\n      \"example\": \"STANDARD\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display title of the event.\",\n      \"example\": \"example-value\"\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\":\
  \ \"The start time of the event as a Unix timestamp in milliseconds.\",\n      \"example\": 1718153645993\n    },\n    \"endTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The end time of the event as a Unix timestamp in milliseconds. Null for open events.\",\n      \"nullable\": true,\n      \"example\": 1718153645993\n    },\n    \"entityId\": {\n      \"$ref\": \"#/components/schemas/EntityStub\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Additional key-value metadata attached to the event.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {}\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the event. OPEN indicates the event is still active; CLOSED indicates it has ended.\",\n      \"enum\": [\n        \"OPEN\",\n        \"CLOSED\"\n      ],\n      \"example\": \"OPEN\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/events-api-v2-event-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: Event
---
