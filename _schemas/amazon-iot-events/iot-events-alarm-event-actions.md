---
description: Contains information about one or more alarm actions.
layout: schema
name: AlarmEventActions
properties_list:
- description: ''
  name: alarmActions
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-alarm-event-actions-schema.json
slug: iot-events-alarm-event-actions
source_filename: iot-events-alarm-event-actions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-event-actions-schema.json\",\n  \"title\": \"AlarmEventActions\",\n  \"description\": \"Contains information about one or more alarm actions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alarmActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmActions\"\n        },\n        {\n          \"description\": \"Specifies one or more supported actions to receive notifications when the alarm state changes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-event-actions-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: AlarmEventActions
---
