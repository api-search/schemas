---
description: A Datadog monitor that watches a metric or check and alerts when thresholds are exceeded
layout: schema
name: Monitor
properties_list:
- description: The unique numeric identifier of the monitor, assigned by Datadog upon creation
  name: id
  type: integer
- description: The type of monitor that determines the query language and alerting behavior
  name: type
  type: string
- description: The monitor query expression using Datadog's query language for the specified monitor type
  name: query
  type: string
- description: A descriptive name for the monitor used for identification in dashboards and notifications
  name: name
  type: string
- description: The notification message body sent when the monitor triggers, supports template variables and @-mentions
  name: message
  type: string
- description: List of tags to associate with the monitor for filtering and organization
  name: tags
  type: array
- description: ''
  name: options
  type: object
- description: The monitor priority level from 1 (highest) to 5 (lowest), used for sorting and filtering
  name: priority
  type: integer
- description: ''
  name: state
  type: object
- description: ''
  name: creator
  type: object
- description: ISO 8601 timestamp when the monitor was created
  name: created
  type: string
- description: ISO 8601 timestamp when the monitor was last modified
  name: modified
  type: string
- description: ISO 8601 timestamp when the monitor was deleted, or null if not deleted
  name: deleted
  type: string
- description: List of role IDs whose members can edit this monitor; empty means all users can edit
  name: restricted_roles
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-monitors-monitor-schema.json
slug: datadog-monitors-monitor
source_filename: datadog-monitors-monitor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-schema.json\",\n  \"title\": \"Monitor\",\n  \"description\": \"A Datadog monitor that watches a metric or check and alerts when thresholds are exceeded\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The unique numeric identifier of the monitor, assigned by Datadog upon creation\",\n      \"example\": 42\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of monitor that determines the query language and alerting behavior\",\n      \"enum\": [\n        \"composite\",\n        \"event alert\",\n        \"log alert\",\n        \"metric alert\",\n        \"process alert\",\n        \"query alert\",\n        \"rum alert\",\n        \"service check\",\n\
  \        \"synthetics alert\",\n        \"trace-analytics alert\",\n        \"slo alert\",\n        \"event-v2 alert\",\n        \"audit alert\",\n        \"ci-pipelines alert\",\n        \"ci-tests alert\",\n        \"error-tracking alert\",\n        \"database-monitoring alert\",\n        \"network-performance alert\"\n      ],\n      \"example\": \"composite\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The monitor query expression using Datadog's query language for the specified monitor type\",\n      \"example\": \"avg:system.cpu.user{*}\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A descriptive name for the monitor used for identification in dashboards and notifications\",\n      \"example\": \"Example Monitor\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The notification message body sent when the monitor triggers, supports template variables and @-mentions\",\n     \
  \ \"example\": \"CPU usage is high on {{host.name}}\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"List of tags to associate with the monitor for filtering and organization\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"options\": {\n      \"$ref\": \"#/components/schemas/MonitorOptions\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"The monitor priority level from 1 (highest) to 5 (lowest), used for sorting and filtering\",\n      \"minimum\": 1,\n      \"maximum\": 5,\n      \"example\": 42\n    },\n    \"state\": {\n      \"$ref\": \"#/components/schemas/MonitorState\"\n    },\n    \"creator\": {\n      \"$ref\": \"#/components/schemas/Creator\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the monitor was created\",\n      \"example\": \"example_value\"\n    },\n    \"modified\": {\n   \
  \   \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the monitor was last modified\",\n      \"example\": \"example_value\"\n    },\n    \"deleted\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"ISO 8601 timestamp when the monitor was deleted, or null if not deleted\",\n      \"example\": \"example_value\"\n    },\n    \"restricted_roles\": {\n      \"type\": \"array\",\n      \"description\": \"List of role IDs whose members can edit this monitor; empty means all users can edit\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"query\",\n    \"name\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: Monitor
---
