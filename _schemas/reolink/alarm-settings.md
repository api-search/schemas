---
description: Motion detection and AI alarm configuration including sensitivity, detection zones, and schedule parameters.
layout: schema
name: Reolink Alarm Settings
properties_list:
- description: Camera channel number
  name: channel
  type: integer
- description: Alarm type
  name: type
  type: string
- description: Enable or disable the alarm (0 = disabled, 1 = enabled)
  name: enable
  type: integer
- description: Sensitivity settings for detection zones
  name: sens
  type: array
- description: Detection area definition as a grid of cells
  name: area
  type: object
- description: Weekly schedule for alarm activation
  name: schedule
  type: object
provider_name: Reolink
provider_slug: reolink
schema_file: json-schema/alarm-settings.json
slug: alarm-settings
source_filename: alarm-settings.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"alarm-settings.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reolink Alarm Settings\",\n  \"description\": \"Motion detection and AI alarm configuration including sensitivity, detection zones, and schedule parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel\": {\n      \"type\": \"integer\",\n      \"description\": \"Camera channel number\",\n      \"minimum\": 0\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Alarm type\",\n      \"enum\": [\"md\", \"people\", \"vehicle\", \"dog_cat\", \"audio\"]\n    },\n    \"enable\": {\n      \"type\": \"integer\",\n      \"description\": \"Enable or disable the alarm (0 = disabled, 1 = enabled)\",\n      \"enum\": [0, 1]\n    },\n    \"sens\": {\n      \"type\": \"array\",\n      \"description\": \"Sensitivity settings for detection zones\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n\
  \          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"Zone identifier\"\n          },\n          \"sensitivity\": {\n            \"type\": \"integer\",\n            \"description\": \"Sensitivity level (0-50)\",\n            \"minimum\": 0,\n            \"maximum\": 50\n          }\n        }\n      }\n    },\n    \"area\": {\n      \"type\": \"object\",\n      \"description\": \"Detection area definition as a grid of cells\",\n      \"properties\": {\n        \"row\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of rows in detection grid\"\n        },\n        \"col\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of columns in detection grid\"\n        },\n        \"table\": {\n          \"type\": \"string\",\n          \"description\": \"Bitmask string defining active detection cells\"\n        }\n      }\n    },\n    \"schedule\": {\n      \"type\": \"object\",\n      \"description\": \"Weekly\
  \ schedule for alarm activation\",\n      \"properties\": {\n        \"enable\": {\n          \"type\": \"integer\",\n          \"enum\": [0, 1]\n        },\n        \"table\": {\n          \"type\": \"string\",\n          \"description\": \"Weekly schedule encoded as a bitmask string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"channel\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/json-schema/alarm-settings.json
tags:
- IoT
- Security Cameras
- Surveillance
- Smart Home
- AI Detection
title: Reolink Alarm Settings
---
