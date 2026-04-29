---
description: The current evaluation state of the monitor across all groups
layout: schema
name: MonitorState
properties_list:
- description: Map of monitor group names to their current state information
  name: groups
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-monitors-monitor-state-schema.json
slug: datadog-monitors-monitor-state
source_filename: datadog-monitors-monitor-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-state-schema.json\",\n  \"title\": \"MonitorState\",\n  \"description\": \"The current evaluation state of the monitor across all groups\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groups\": {\n      \"type\": \"object\",\n      \"description\": \"Map of monitor group names to their current state information\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/MonitorGroupState\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-state-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MonitorState
---
