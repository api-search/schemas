---
description: Represents a cron job monitor in Sentry. Monitors track scheduled tasks and alert when check-ins are missed or fail, providing visibility into the health of background jobs and cron tasks.
layout: schema
name: Sentry Monitor
properties_list:
- description: The unique identifier of the monitor.
  name: id
  type: string
- description: The URL-friendly slug of the monitor.
  name: slug
  type: string
- description: The human-readable name of the monitor.
  name: name
  type: string
- description: The type of monitor.
  name: type
  type: string
- description: The monitor's schedule configuration.
  name: config
  type: object
- description: The current status of the monitor.
  name: status
  type: string
- description: When the monitor was created.
  name: dateCreated
  type: string
- description: The project associated with this monitor.
  name: project
  type: object
- description: Environment-specific monitor statuses.
  name: environments
  type: array
provider_name: Sentry
provider_slug: sentry-system
schema_file: json-schema/sentry-monitor-schema.json
slug: sentry-monitor
source_filename: sentry-monitor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://sentry.io/schemas/monitor.json\",\n  \"title\": \"Sentry Monitor\",\n  \"description\": \"Represents a cron job monitor in Sentry. Monitors track scheduled tasks and alert when check-ins are missed or fail, providing visibility into the health of background jobs and cron tasks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the monitor.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly slug of the monitor.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the monitor.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of monitor.\",\n      \"enum\": [\"cron_job\"]\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"\
  The monitor's schedule configuration.\",\n      \"properties\": {\n        \"schedule_type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of schedule.\",\n          \"enum\": [\"crontab\", \"interval\"]\n        },\n        \"schedule\": {\n          \"description\": \"The schedule definition. A crontab string or interval array.\",\n          \"oneOf\": [\n            {\n              \"type\": \"string\",\n              \"description\": \"Crontab expression (e.g., '*/5 * * * *').\"\n            },\n            {\n              \"type\": \"array\",\n              \"description\": \"Interval as [value, unit] (e.g., [1, 'hour']).\",\n              \"items\": {}\n            }\n          ]\n        },\n        \"checkin_margin\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Margin of minutes before a check-in is marked as missed.\"\n        },\n        \"max_runtime\": {\n          \"type\": [\"integer\", \"null\"],\n        \
  \  \"description\": \"Maximum runtime in minutes before a check-in is marked as timed out.\"\n        },\n        \"timezone\": {\n          \"type\": \"string\",\n          \"description\": \"The timezone for the schedule (e.g., UTC, America/New_York).\"\n        }\n      },\n      \"required\": [\"schedule_type\", \"schedule\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the monitor.\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the monitor was created.\"\n    },\n    \"project\": {\n      \"type\": \"object\",\n      \"description\": \"The project associated with this monitor.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"slug\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"environments\": {\n      \"\
  type\": \"array\",\n      \"description\": \"Environment-specific monitor statuses.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\"\n          },\n          \"lastCheckIn\": {\n            \"type\": [\"string\", \"null\"],\n            \"format\": \"date-time\"\n          },\n          \"nextCheckIn\": {\n            \"type\": [\"string\", \"null\"],\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\", \"config\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/json-schema/sentry-monitor-schema.json
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
title: Sentry Monitor
---
