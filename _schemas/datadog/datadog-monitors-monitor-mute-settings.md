---
description: Settings for muting a monitor including scope and expiration
layout: schema
name: MonitorMuteSettings
properties_list:
- description: The scope expression specifying which monitor groups to mute (e.g., env:prod, host:web-01)
  name: scope
  type: string
- description: Unix timestamp in seconds when the mute expires; omit for indefinite mute
  name: end
  type: integer
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-monitors-monitor-mute-settings-schema.json
slug: datadog-monitors-monitor-mute-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-mute-settings-schema.json\",\n  \"title\": \"MonitorMuteSettings\",\n  \"description\": \"Settings for muting a monitor including scope and expiration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"The scope expression specifying which monitor groups to mute (e.g., env:prod, host:web-01)\",\n      \"example\": \"example_value\"\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unix timestamp in seconds when the mute expires; omit for indefinite mute\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-mute-settings-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MonitorMuteSettings
---
