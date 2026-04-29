---
description: Defines when your alarm is invoked.
layout: schema
name: AlarmRule
properties_list:
- description: ''
  name: simpleRule
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-alarm-rule-schema.json
slug: iot-events-alarm-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-rule-schema.json\",\n  \"title\": \"AlarmRule\",\n  \"description\": \"Defines when your alarm is invoked.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"simpleRule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimpleRule\"\n        },\n        {\n          \"description\": \"A rule that compares an input property value to a threshold value with a comparison operator.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-rule-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: AlarmRule
---
