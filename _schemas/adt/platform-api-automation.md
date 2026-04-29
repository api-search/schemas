---
description: An automation rule or smart home scene.
layout: schema
name: Automation
properties_list:
- description: Unique identifier of the automation.
  name: id
  type: string
- description: Display name of the automation.
  name: name
  type: string
- description: What triggers this automation.
  name: trigger
  type: string
- description: Whether the automation is currently active.
  name: enabled
  type: boolean
- description: List of actions performed by this automation.
  name: actions
  type: array
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-automation-schema.json
slug: platform-api-automation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-automation-schema.json\",\n  \"title\": \"Automation\",\n  \"description\": \"An automation rule or smart home scene.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the automation.\",\n      \"example\": \"auto-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the automation.\",\n      \"example\": \"Arm Away at Night\"\n    },\n    \"trigger\": {\n      \"type\": \"string\",\n      \"description\": \"What triggers this automation.\",\n      \"enum\": [\n        \"schedule\",\n        \"alarm\",\n        \"sensor\",\n        \"geofence\",\n        \"manual\"\n      ],\n      \"example\": \"schedule\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n\
  \      \"description\": \"Whether the automation is currently active.\",\n      \"example\": true\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"description\": \"List of actions performed by this automation.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-automation-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: Automation
---
