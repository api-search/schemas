---
description: An alert monitor defines conditions for monitoring instance executions and triggering notifications when those conditions are met.
layout: schema
name: Prismatic Alert Monitor
properties_list:
- description: Unique identifier for the alert monitor
  name: id
  type: string
- description: Name of the alert monitor
  name: name
  type: string
- description: Whether the alert is currently in a triggered state
  name: triggered
  type: boolean
- description: Type of trigger condition for the alert
  name: triggerType
  type: string
- description: The instance this alert monitor is attached to
  name: instance
  type: object
- description: Alert groups that receive notifications from this monitor
  name: groups
  type: array
- description: Duration threshold in seconds for duration-based triggers
  name: durationSecondsCondition
  type: integer
- description: Log severity level threshold for severity-based triggers
  name: logSeverityLevelCondition
  type: integer
- description: Minutes past expected schedule before triggering overdue alert
  name: executionOverdueMinutes
  type: integer
- description: Timestamp when the alert monitor was created
  name: createdAt
  type: string
- description: Timestamp when the alert monitor was last updated
  name: updatedAt
  type: string
provider_name: Prismatic
provider_slug: prismatic
schema_file: json-schema/alert-monitor.json
slug: alert-monitor
source_filename: alert-monitor.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/alert-monitor.json\",\n  \"title\": \"Prismatic Alert Monitor\",\n  \"description\": \"An alert monitor defines conditions for monitoring instance executions and triggering notifications when those conditions are met.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the alert monitor\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the alert monitor\"\n    },\n    \"triggered\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the alert is currently in a triggered state\"\n    },\n    \"triggerType\": {\n      \"type\": \"string\",\n      \"enum\": [\"execution_failed\", \"execution_overdue\", \"execution_duration_matched\"\
  , \"log_severity_matched\", \"connection_error\"],\n      \"description\": \"Type of trigger condition for the alert\"\n    },\n    \"instance\": {\n      \"$ref\": \"instance.json\",\n      \"description\": \"The instance this alert monitor is attached to\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"Alert groups that receive notifications from this monitor\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"durationSecondsCondition\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration threshold in seconds for duration-based triggers\"\n    },\n    \"logSeverityLevelCondition\": {\n      \"type\": \"integer\",\n      \"description\": \"Log severity level threshold for severity-based triggers\"\n    },\n    \"executionOverdueMinutes\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Minutes past expected schedule before triggering overdue alert\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the alert monitor was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the alert monitor was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/alert-monitor.json
tags:
- Embedded iPaaS
- Integrations
- Workflows
title: Prismatic Alert Monitor
---
