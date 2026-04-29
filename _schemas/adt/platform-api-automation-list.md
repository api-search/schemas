---
description: List of automation rules.
layout: schema
name: AutomationList
properties_list:
- description: Array of automation rules.
  name: automations
  type: array
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-automation-list-schema.json
slug: platform-api-automation-list
source_filename: platform-api-automation-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-automation-list-schema.json\",\n  \"title\": \"AutomationList\",\n  \"description\": \"List of automation rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"automations\": {\n      \"type\": \"array\",\n      \"description\": \"Array of automation rules.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An automation rule or smart home scene.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier of the automation.\",\n            \"example\": \"auto-001\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name of the automation.\",\n            \"example\": \"Arm Away at Night\"\n          },\n          \"trigger\": {\n\
  \            \"type\": \"string\",\n            \"description\": \"What triggers this automation.\",\n            \"enum\": [\n              \"schedule\",\n              \"alarm\",\n              \"sensor\",\n              \"geofence\",\n              \"manual\"\n            ],\n            \"example\": \"schedule\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the automation is currently active.\",\n            \"example\": true\n          },\n          \"actions\": {\n            \"type\": \"array\",\n            \"description\": \"List of actions performed by this automation.\",\n            \"items\": {\n              \"type\": \"object\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-automation-list-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: AutomationList
---
