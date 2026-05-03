---
description: Represents an alert rule in Sentry. Alert rules define conditions that trigger notifications when error or performance thresholds are breached. Includes both metric alert rules and issue alert rules.
layout: schema
name: Sentry Alert Rule
properties_list:
- description: The unique identifier of the alert rule.
  name: id
  type: string
- description: The name of the alert rule.
  name: name
  type: string
- description: The aggregation function for metric alerts (e.g., count(), p50(transaction.duration)).
  name: aggregate
  type: string
- description: The dataset to query (e.g., events, transactions, sessions).
  name: dataset
  type: string
- description: An optional Sentry search query to filter events.
  name: query
  type: string
- description: The time window in minutes to evaluate the alert.
  name: timeWindow
  type: integer
- description: The environment to filter by.
  name: environment
  type:
  - string
  - 'null'
- description: The project slugs the alert applies to.
  name: projects
  type: array
- description: The trigger conditions for the alert.
  name: triggers
  type: array
- description: The owner of the alert (user:id or team:id).
  name: owner
  type:
  - string
  - 'null'
- description: When the alert rule was created.
  name: dateCreated
  type: string
- description: When the alert rule was last modified.
  name: dateModified
  type: string
provider_name: Sentry
provider_slug: sentry-system
schema_file: json-schema/sentry-alert-rule-schema.json
slug: sentry-alert-rule
source_filename: sentry-alert-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://sentry.io/schemas/alert-rule.json\",\n  \"title\": \"Sentry Alert Rule\",\n  \"description\": \"Represents an alert rule in Sentry. Alert rules define conditions that trigger notifications when error or performance thresholds are breached. Includes both metric alert rules and issue alert rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the alert rule.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the alert rule.\"\n    },\n    \"aggregate\": {\n      \"type\": \"string\",\n      \"description\": \"The aggregation function for metric alerts (e.g., count(), p50(transaction.duration)).\"\n    },\n    \"dataset\": {\n      \"type\": \"string\",\n      \"description\": \"The dataset to query (e.g., events, transactions, sessions).\"\n    },\n\
  \    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"An optional Sentry search query to filter events.\"\n    },\n    \"timeWindow\": {\n      \"type\": \"integer\",\n      \"description\": \"The time window in minutes to evaluate the alert.\"\n    },\n    \"environment\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The environment to filter by.\"\n    },\n    \"projects\": {\n      \"type\": \"array\",\n      \"description\": \"The project slugs the alert applies to.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"triggers\": {\n      \"type\": \"array\",\n      \"description\": \"The trigger conditions for the alert.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"Trigger label (e.g., critical, warning).\"\n          },\n\
  \          \"alertThreshold\": {\n            \"type\": \"number\",\n            \"description\": \"The threshold value that triggers the alert.\"\n          },\n          \"resolveThreshold\": {\n            \"type\": [\"number\", \"null\"],\n            \"description\": \"The threshold value that resolves the alert.\"\n          },\n          \"thresholdType\": {\n            \"type\": \"integer\",\n            \"description\": \"0 for above, 1 for below.\"\n          },\n          \"actions\": {\n            \"type\": \"array\",\n            \"description\": \"Actions to perform when triggered.\",\n            \"items\": {\n              \"type\": \"object\"\n            }\n          }\n        }\n      }\n    },\n    \"owner\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The owner of the alert (user:id or team:id).\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the alert rule was\
  \ created.\"\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the alert rule was last modified.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/json-schema/sentry-alert-rule-schema.json
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
title: Sentry Alert Rule
---
