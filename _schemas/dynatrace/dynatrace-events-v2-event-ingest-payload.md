---
description: The payload for ingesting a custom event into Dynatrace. All events require at least an eventType and title. Custom events can target specific entities, include a time window, and carry additional metadata as key-value properties.
layout: schema
name: EventIngestPayload
properties_list:
- description: The type of the custom event. Determines how the event is categorized and whether it triggers alerts or problem detection.
  name: eventType
  type: string
- description: 'How long the event remains open, in minutes, if no endTime is specified. Range: 1 to 60 minutes. If not specified, the event closes after a short default duration.'
  name: timeout
  type: integer
- description: The entity selector specifying which entities the event should be associated with. For example, type(SERVICE),tag(production). Required for most event types.
  name: entitySelector
  type: string
- description: The title of the event. This is displayed in the Dynatrace UI and in problem notifications. Required.
  name: title
  type: string
- description: The start time of the event as a Unix timestamp in milliseconds. If not specified, defaults to the current time.
  name: startTime
  type: integer
- description: The end time of the event as a Unix timestamp in milliseconds. If specified, creates a closed event covering the time range.
  name: endTime
  type: integer
- description: Additional key-value metadata to attach to the event. Maximum of 30 key-value pairs. Keys and values must be strings.
  name: properties
  type: object
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-events-v2-event-ingest-payload-schema.json
slug: dynatrace-events-v2-event-ingest-payload
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The payload for ingesting a custom event into Dynatrace. All events require at least an eventType and title. Custom events can target specific entities, include a time window, and carry additional metadata as key-value properties.\",\n  \"properties\": {\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the custom event. Determines how the event is categorized and whether it triggers alerts or problem detection.\",\n      \"example\": \"AVAILABILITY_EVENT\",\n      \"enum\": [\n        \"AVAILABILITY_EVENT\",\n        \"CUSTOM_ALERT\",\n        \"CUSTOM_ANNOTATION\",\n        \"CUSTOM_CONFIGURATION\",\n        \"CUSTOM_DEPLOYMENT\",\n        \"ERROR_EVENT\",\n        \"MARKED_FOR_TERMINATION\",\n        \"PERFORMANCE_EVENT\",\n        \"RESOURCE_CONTENTION_EVENT\"\n      ]\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"How long the event remains open,\
  \ in minutes, if no endTime is specified. Range: 1 to 60 minutes. If not specified, the event closes after a short default duration.\",\n      \"example\": 1718153645993\n    },\n    \"entitySelector\": {\n      \"type\": \"string\",\n      \"description\": \"The entity selector specifying which entities the event should be associated with. For example, type(SERVICE),tag(production). Required for most event types.\",\n      \"example\": \"type(SERVICE)\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the event. This is displayed in the Dynatrace UI and in problem notifications. Required.\",\n      \"example\": \"example-value\"\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"description\": \"The start time of the event as a Unix timestamp in milliseconds. If not specified, defaults to the current time.\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993\n    },\n    \"endTime\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"The end time of the event as a Unix timestamp in milliseconds. If specified, creates a closed event covering the time range.\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Additional key-value metadata to attach to the event. Maximum of 30 key-value pairs. Keys and values must be strings.\",\n      \"example\": {}\n    }\n  },\n  \"required\": [\n    \"eventType\",\n    \"title\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventIngestPayload\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-events-v2-event-ingest-payload-schema.json
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
title: EventIngestPayload
---
