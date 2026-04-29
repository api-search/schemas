---
description: Settings for unmuting a monitor including optional scope
layout: schema
name: MonitorUnmuteSettings
properties_list:
- description: The scope expression specifying which monitor groups to unmute; omit to unmute all groups
  name: scope
  type: string
- description: When true, unmutes all scopes including those previously muted with different scope expressions
  name: all_scopes
  type: boolean
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-monitors-monitor-unmute-settings-schema.json
slug: datadog-monitors-monitor-unmute-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-unmute-settings-schema.json\",\n  \"title\": \"MonitorUnmuteSettings\",\n  \"description\": \"Settings for unmuting a monitor including optional scope\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"The scope expression specifying which monitor groups to unmute; omit to unmute all groups\",\n      \"example\": \"example_value\"\n    },\n    \"all_scopes\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, unmutes all scopes including those previously muted with different scope expressions\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-monitors-monitor-unmute-settings-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MonitorUnmuteSettings
---
