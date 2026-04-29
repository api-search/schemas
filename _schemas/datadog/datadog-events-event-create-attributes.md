---
description: The attributes for a new event to be created
layout: schema
name: EventCreateAttributes
properties_list:
- description: The event title displayed in the Events Explorer (max 100 characters)
  name: title
  type: string
- description: The event body text with additional details about the event (max 4000 characters)
  name: message
  type: string
- description: Unix timestamp in seconds for when the event occurred; defaults to current time if not specified
  name: timestamp
  type: integer
- description: The event priority level for filtering and sorting in the Events Explorer
  name: priority
  type: string
- description: The hostname to associate with this event for infrastructure correlation
  name: host
  type: string
- description: List of tags to apply to the event in key:value format for filtering
  name: tags
  type: array
- description: The alert type category for visual display in the Events Explorer
  name: alert_type
  type: string
- description: An arbitrary string used to group related events into a rollup (max 100 characters)
  name: aggregation_key
  type: string
- description: The source technology or integration that generated this event (e.g., aws, chef, nagios)
  name: source_type_name
  type: string
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-events-event-create-attributes-schema.json
slug: datadog-events-event-create-attributes
source_filename: datadog-events-event-create-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-create-attributes-schema.json\",\n  \"title\": \"EventCreateAttributes\",\n  \"description\": \"The attributes for a new event to be created\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The event title displayed in the Events Explorer (max 100 characters)\",\n      \"maxLength\": 100,\n      \"example\": \"Example Monitor\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The event body text with additional details about the event (max 4000 characters)\",\n      \"maxLength\": 4000,\n      \"example\": \"CPU usage is high on {{host.name}}\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unix timestamp in seconds\
  \ for when the event occurred; defaults to current time if not specified\",\n      \"example\": 42\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"The event priority level for filtering and sorting in the Events Explorer\",\n      \"enum\": [\n        \"normal\",\n        \"low\"\n      ],\n      \"default\": \"normal\",\n      \"example\": \"normal\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname to associate with this event for infrastructure correlation\",\n      \"example\": \"example_value\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"List of tags to apply to the event in key:value format for filtering\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"alert_type\": {\n      \"type\": \"string\",\n      \"description\": \"The alert type category for visual display in the Events Explorer\",\n      \"enum\": [\n        \"error\",\n        \"\
  warning\",\n        \"info\",\n        \"success\",\n        \"user_update\",\n        \"recommendation\",\n        \"snapshot\"\n      ],\n      \"default\": \"info\",\n      \"example\": \"error\"\n    },\n    \"aggregation_key\": {\n      \"type\": \"string\",\n      \"description\": \"An arbitrary string used to group related events into a rollup (max 100 characters)\",\n      \"maxLength\": 100,\n      \"example\": \"example_value\"\n    },\n    \"source_type_name\": {\n      \"type\": \"string\",\n      \"description\": \"The source technology or integration that generated this event (e.g., aws, chef, nagios)\",\n      \"example\": \"Example Monitor\"\n    }\n  },\n  \"required\": [\n    \"title\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-events-event-create-attributes-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: EventCreateAttributes
---
