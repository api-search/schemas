---
description: A single log entry to submit to Datadog
layout: schema
name: HTTPLogItem
properties_list:
- description: The message content of the log entry. This field is required and indexed for search.
  name: message
  type: string
- description: The name of the host that generated the log entry
  name: hostname
  type: string
- description: The name of the application or service that generated the log
  name: service
  type: string
- description: The source technology of the log (e.g., nginx, redis, java) used for automatic processing
  name: ddsource
  type: string
- description: Comma-separated list of tags to apply to the log entry in key:value format
  name: ddtags
  type: string
- description: The severity or log level of the event (e.g., info, warning, error, critical)
  name: status
  type: string
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-logs-http-log-item-schema.json
slug: datadog-logs-http-log-item
source_filename: datadog-logs-http-log-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-http-log-item-schema.json\",\n  \"title\": \"HTTPLogItem\",\n  \"description\": \"A single log entry to submit to Datadog\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The message content of the log entry. This field is required and indexed for search.\",\n      \"example\": \"CPU usage is high on {{host.name}}\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the host that generated the log entry\",\n      \"example\": \"Example Monitor\"\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application or service that generated the log\",\n      \"example\": \"example_value\"\n    },\n    \"ddsource\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The source technology of the log (e.g., nginx, redis, java) used for automatic processing\",\n      \"example\": \"example_value\"\n    },\n    \"ddtags\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of tags to apply to the log entry in key:value format\",\n      \"example\": \"env:production\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The severity or log level of the event (e.g., info, warning, error, critical)\",\n      \"enum\": [\n        \"emerg\",\n        \"alert\",\n        \"critical\",\n        \"error\",\n        \"warning\",\n        \"notice\",\n        \"info\",\n        \"debug\"\n      ],\n      \"example\": \"emerg\"\n    }\n  },\n  \"required\": [\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-http-log-item-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: HTTPLogItem
---
