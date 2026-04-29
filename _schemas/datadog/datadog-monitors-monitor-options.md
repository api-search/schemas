---
description: Configuration options for a monitor controlling evaluation, notification, and recovery behavior
layout: schema
name: MonitorOptions
properties_list:
- description: ''
  name: thresholds
  type: object
- description: Whether to send a notification when there is no data for the monitored metric
  name: notify_no_data
  type: boolean
- description: The number of minutes after which the monitor reports no data (minimum 2x the evaluation timeframe)
  name: no_data_timeframe
  type: integer
- description: Whether the monitor requires a full evaluation window of data before alerting
  name: require_full_window
  type: boolean
- description: Whether to send notifications to auditors when the monitor is changed
  name: notify_audit
  type: boolean
- description: The number of minutes between re-notifications while the monitor remains in an alert state (0 to disable)
  name: renotify_interval
  type: integer
- description: Monitor status types that trigger re-notification messages
  name: renotify_statuses
  type: array
- description: The message to include with re-notification alerts instead of the main message
  name: escalation_message
  type: string
- description: The number of hours after which an automatically resolving alert times out
  name: timeout_h
  type: integer
- description: The time in seconds to delay evaluation, used to ensure all data arrives before checking thresholds
  name: evaluation_delay
  type: integer
- description: The number of seconds to delay notification for new monitor groups to allow transient issues to resolve
  name: new_group_delay
  type: integer
- description: Whether to include group scope tags in notification subject and body
  name: include_tags
  type: boolean
- description: Map of monitor scopes to Unix timestamps indicating when each scope's mute expires (0 for indefinite)
  name: silenced
  type: object
- description: Aggregation settings used for anomaly and outlier monitors
  name: aggregation
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-monitors-monitor-options-schema.json
slug: datadog-monitors-monitor-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-options-schema.json\",\n  \"title\": \"MonitorOptions\",\n  \"description\": \"Configuration options for a monitor controlling evaluation, notification, and recovery behavior\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thresholds\": {\n      \"$ref\": \"#/components/schemas/MonitorThresholds\"\n    },\n    \"notify_no_data\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to send a notification when there is no data for the monitored metric\",\n      \"default\": false,\n      \"example\": true\n    },\n    \"no_data_timeframe\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of minutes after which the monitor reports no data (minimum 2x the evaluation timeframe)\",\n      \"example\": 42\n    },\n    \"require_full_window\": {\n   \
  \   \"type\": \"boolean\",\n      \"description\": \"Whether the monitor requires a full evaluation window of data before alerting\",\n      \"example\": true\n    },\n    \"notify_audit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to send notifications to auditors when the monitor is changed\",\n      \"example\": true\n    },\n    \"renotify_interval\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of minutes between re-notifications while the monitor remains in an alert state (0 to disable)\",\n      \"example\": 42\n    },\n    \"renotify_statuses\": {\n      \"type\": \"array\",\n      \"description\": \"Monitor status types that trigger re-notification messages\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"alert\",\n          \"warn\",\n          \"no data\"\n        ]\n      }\n    },\n    \"escalation_message\": {\n      \"type\": \"string\",\n      \"description\": \"The message to include\
  \ with re-notification alerts instead of the main message\",\n      \"example\": \"CPU usage is high on {{host.name}}\"\n    },\n    \"timeout_h\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of hours after which an automatically resolving alert times out\",\n      \"example\": 42\n    },\n    \"evaluation_delay\": {\n      \"type\": \"integer\",\n      \"description\": \"The time in seconds to delay evaluation, used to ensure all data arrives before checking thresholds\",\n      \"example\": 42\n    },\n    \"new_group_delay\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of seconds to delay notification for new monitor groups to allow transient issues to resolve\",\n      \"example\": 42\n    },\n    \"include_tags\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include group scope tags in notification subject and body\",\n      \"default\": true,\n      \"example\": true\n    },\n    \"silenced\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Map of monitor scopes to Unix timestamps indicating when each scope's mute expires (0 for indefinite)\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"nullable\": true\n      }\n    },\n    \"aggregation\": {\n      \"type\": \"object\",\n      \"description\": \"Aggregation settings used for anomaly and outlier monitors\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of aggregation function applied to the metric\"\n        },\n        \"metric\": {\n          \"type\": \"string\",\n          \"description\": \"The metric name used in the aggregation\"\n        },\n        \"group_by\": {\n          \"type\": \"string\",\n          \"description\": \"The tag key to group the aggregation by\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-options-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MonitorOptions
---
