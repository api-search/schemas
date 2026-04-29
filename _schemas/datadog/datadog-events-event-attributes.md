---
description: The attributes of an event returned from the Events Explorer
layout: schema
name: EventAttributes
properties_list:
- description: The event title as displayed in the Events Explorer
  name: title
  type: string
- description: The event body text containing details about the event
  name: message
  type: string
- description: ISO 8601 timestamp when the event was recorded
  name: timestamp
  type: string
- description: The event priority level
  name: priority
  type: string
- description: The hostname associated with this event
  name: host
  type: string
- description: List of tags associated with the event in key:value format
  name: tags
  type: array
- description: The alert type category for visual display
  name: alert_type
  type: string
- description: The arbitrary string used to group related events into a rollup
  name: aggregation_key
  type: string
- description: The source technology or integration that generated this event
  name: source_type_name
  type: string
- description: The event status (active or expired)
  name: status
  type: string
- description: Custom key-value attributes associated with the event
  name: attributes
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-events-event-attributes-schema.json
slug: datadog-events-event-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-attributes-schema.json\",\n  \"title\": \"EventAttributes\",\n  \"description\": \"The attributes of an event returned from the Events Explorer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The event title as displayed in the Events Explorer\",\n      \"example\": \"Example Monitor\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The event body text containing details about the event\",\n      \"example\": \"CPU usage is high on {{host.name}}\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the event was recorded\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"priority\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The event priority level\",\n      \"enum\": [\n        \"normal\",\n        \"low\"\n      ],\n      \"example\": \"normal\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname associated with this event\",\n      \"example\": \"example_value\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"List of tags associated with the event in key:value format\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"alert_type\": {\n      \"type\": \"string\",\n      \"description\": \"The alert type category for visual display\",\n      \"enum\": [\n        \"error\",\n        \"warning\",\n        \"info\",\n        \"success\",\n        \"user_update\",\n        \"recommendation\",\n        \"snapshot\"\n      ],\n      \"example\": \"error\"\n    },\n    \"aggregation_key\": {\n      \"type\": \"string\",\n      \"description\": \"The arbitrary\
  \ string used to group related events into a rollup\",\n      \"example\": \"example_value\"\n    },\n    \"source_type_name\": {\n      \"type\": \"string\",\n      \"description\": \"The source technology or integration that generated this event\",\n      \"example\": \"Example Monitor\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The event status (active or expired)\",\n      \"example\": \"OK\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Custom key-value attributes associated with the event\",\n      \"additionalProperties\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-attributes-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: EventAttributes
---
