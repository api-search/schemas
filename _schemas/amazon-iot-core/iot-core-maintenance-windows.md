---
description: MaintenanceWindows schema
layout: schema
name: MaintenanceWindows
properties_list: []
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-maintenance-windows-schema.json
slug: iot-core-maintenance-windows
source_filename: iot-core-maintenance-windows-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-maintenance-windows-schema.json\",\n  \"title\": \"MaintenanceWindows\",\n  \"description\": \"MaintenanceWindows schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"startTime\",\n      \"durationInMinutes\"\n    ],\n    \"properties\": {\n      \"startTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CronExpression\"\n          },\n          {\n            \"description\": \"Displays the start time of the next maintenance window.\"\n          }\n        ]\n      },\n      \"durationInMinutes\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DurationInMinutes\"\n          },\n          {\n            \"description\": \"Displays the duration of the next maintenance\
  \ window.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An optional configuration within the <code>SchedulingConfig</code> to setup a recurring maintenance window with a predetermined start time and duration for the rollout of a job document to all devices in a target group for a job.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-maintenance-windows-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: MaintenanceWindows
---
