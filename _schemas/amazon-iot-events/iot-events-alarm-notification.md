---
description: Contains information about one or more notification actions.
layout: schema
name: AlarmNotification
properties_list:
- description: ''
  name: notificationActions
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-alarm-notification-schema.json
slug: iot-events-alarm-notification
source_filename: iot-events-alarm-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-notification-schema.json\",\n  \"title\": \"AlarmNotification\",\n  \"description\": \"Contains information about one or more notification actions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationActions\"\n        },\n        {\n          \"description\": \"Contains the notification settings of an alarm model. The settings apply to all alarms that were created based on this alarm model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-notification-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: AlarmNotification
---
