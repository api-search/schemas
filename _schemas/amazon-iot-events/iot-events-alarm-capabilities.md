---
description: Contains the configuration information of alarm state changes.
layout: schema
name: AlarmCapabilities
properties_list:
- description: ''
  name: initializationConfiguration
  type: object
- description: ''
  name: acknowledgeFlow
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-alarm-capabilities-schema.json
slug: iot-events-alarm-capabilities
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-capabilities-schema.json\",\n  \"title\": \"AlarmCapabilities\",\n  \"description\": \"Contains the configuration information of alarm state changes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"initializationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InitializationConfiguration\"\n        },\n        {\n          \"description\": \"Specifies the default alarm state. The configuration applies to all alarms that were created based on this alarm model.\"\n        }\n      ]\n    },\n    \"acknowledgeFlow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AcknowledgeFlow\"\n        },\n        {\n          \"description\": \"Specifies whether to get notified for alarm state changes.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-capabilities-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: AlarmCapabilities
---
