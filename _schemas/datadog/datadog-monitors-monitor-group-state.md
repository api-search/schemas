---
description: The state of a single monitor group (a unique combination of tag values)
layout: schema
name: MonitorGroupState
properties_list:
- description: The current alert status for this monitor group
  name: status
  type: string
- description: The name of the monitor group, represented as a comma-separated list of tag:value pairs
  name: name
  type: string
- description: Unix timestamp in seconds of the last time this group triggered an alert
  name: last_triggered_ts
  type: integer
- description: Unix timestamp in seconds of the last time a notification was sent for this group
  name: last_notified_ts
  type: integer
- description: Unix timestamp in seconds of the last time this group resolved from an alert state
  name: last_resolved_ts
  type: integer
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-monitors-monitor-group-state-schema.json
slug: datadog-monitors-monitor-group-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-group-state-schema.json\",\n  \"title\": \"MonitorGroupState\",\n  \"description\": \"The state of a single monitor group (a unique combination of tag values)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current alert status for this monitor group\",\n      \"enum\": [\n        \"Alert\",\n        \"Ignored\",\n        \"No Data\",\n        \"OK\",\n        \"Skipped\",\n        \"Unknown\",\n        \"Warn\"\n      ],\n      \"example\": \"Alert\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the monitor group, represented as a comma-separated list of tag:value pairs\",\n      \"example\": \"Example Monitor\"\n    },\n    \"last_triggered_ts\": {\n      \"type\"\
  : \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unix timestamp in seconds of the last time this group triggered an alert\",\n      \"example\": 42\n    },\n    \"last_notified_ts\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unix timestamp in seconds of the last time a notification was sent for this group\",\n      \"example\": 42\n    },\n    \"last_resolved_ts\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unix timestamp in seconds of the last time this group resolved from an alert state\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-group-state-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MonitorGroupState
---
