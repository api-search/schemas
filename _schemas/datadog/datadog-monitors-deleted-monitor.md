---
description: Response returned after successfully deleting a monitor
layout: schema
name: DeletedMonitor
properties_list:
- description: The ID of the monitor that was deleted
  name: deleted_monitor_id
  type: integer
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-monitors-deleted-monitor-schema.json
slug: datadog-monitors-deleted-monitor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-deleted-monitor-schema.json\",\n  \"title\": \"DeletedMonitor\",\n  \"description\": \"Response returned after successfully deleting a monitor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deleted_monitor_id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The ID of the monitor that was deleted\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-deleted-monitor-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: DeletedMonitor
---
