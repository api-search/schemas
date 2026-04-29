---
description: A single log event returned from a search query
layout: schema
name: Log
properties_list:
- description: The unique identifier of the log event
  name: id
  type: string
- description: The type of the resource (always 'log')
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-logs-log-schema.json
slug: datadog-logs-log
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-log-schema.json\",\n  \"title\": \"Log\",\n  \"description\": \"A single log event returned from a search query\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the log event\",\n      \"example\": \"abc-123-def\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource (always 'log')\",\n      \"example\": \"metric alert\"\n    },\n    \"attributes\": {\n      \"$ref\": \"#/components/schemas/LogAttributes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-log-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: Log
---
