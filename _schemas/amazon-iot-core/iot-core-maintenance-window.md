---
description: An optional configuration within the <code>SchedulingConfig</code> to setup a recurring maintenance window with a predetermined start time and duration for the rollout of a job document to all devices in a target group for a job.
layout: schema
name: MaintenanceWindow
properties_list:
- description: ''
  name: startTime
  type: object
- description: ''
  name: durationInMinutes
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-maintenance-window-schema.json
slug: iot-core-maintenance-window
source_filename: iot-core-maintenance-window-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-maintenance-window-schema.json\",\n  \"title\": \"MaintenanceWindow\",\n  \"description\": \"An optional configuration within the <code>SchedulingConfig</code> to setup a recurring maintenance window with a predetermined start time and duration for the rollout of a job document to all devices in a target group for a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CronExpression\"\n        },\n        {\n          \"description\": \"Displays the start time of the next maintenance window.\"\n        }\n      ]\n    },\n    \"durationInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInMinutes\"\n        },\n        {\n          \"description\": \"\
  Displays the duration of the next maintenance window.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"startTime\",\n    \"durationInMinutes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-maintenance-window-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: MaintenanceWindow
---
