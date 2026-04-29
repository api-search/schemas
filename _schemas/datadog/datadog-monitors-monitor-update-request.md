---
description: Request body for updating an existing monitor configuration
layout: schema
name: MonitorUpdateRequest
properties_list:
- description: The type of the monitor (changing type may reset other settings)
  name: type
  type: string
- description: The updated monitor query expression
  name: query
  type: string
- description: The updated descriptive name for the monitor
  name: name
  type: string
- description: The updated notification message body
  name: message
  type: string
- description: The updated list of tags to associate with the monitor
  name: tags
  type: array
- description: ''
  name: options
  type: object
- description: The updated priority level (1 highest to 5 lowest)
  name: priority
  type: integer
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-monitors-monitor-update-request-schema.json
slug: datadog-monitors-monitor-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-update-request-schema.json\",\n  \"title\": \"MonitorUpdateRequest\",\n  \"description\": \"Request body for updating an existing monitor configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the monitor (changing type may reset other settings)\",\n      \"example\": \"metric alert\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The updated monitor query expression\",\n      \"example\": \"avg:system.cpu.user{*}\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The updated descriptive name for the monitor\",\n      \"example\": \"Example Monitor\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The updated notification message body\",\n      \"example\": \"CPU usage is high on {{host.name}}\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"The updated list of tags to associate with the monitor\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"options\": {\n      \"$ref\": \"#/components/schemas/MonitorOptions\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"The updated priority level (1 highest to 5 lowest)\",\n      \"minimum\": 1,\n      \"maximum\": 5,\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-update-request-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MonitorUpdateRequest
---
