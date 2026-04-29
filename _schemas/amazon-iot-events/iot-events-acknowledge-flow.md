---
description: Specifies whether to get notified for alarm state changes.
layout: schema
name: AcknowledgeFlow
properties_list:
- description: ''
  name: enabled
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-acknowledge-flow-schema.json
slug: iot-events-acknowledge-flow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-acknowledge-flow-schema.json\",\n  \"title\": \"AcknowledgeFlow\",\n  \"description\": \"Specifies whether to get notified for alarm state changes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AcknowledgeFlowEnabled\"\n        },\n        {\n          \"description\": \"The value must be <code>TRUE</code> or <code>FALSE</code>. If <code>TRUE</code>, you receive a notification when the alarm state changes. You must choose to acknowledge the notification before the alarm state can return to <code>NORMAL</code>. If <code>FALSE</code>, you won't receive notifications. The alarm automatically changes to the <code>NORMAL</code> state when the input property value returns to the specified range.\"\n\
  \        }\n      ]\n    }\n  },\n  \"required\": [\n    \"enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-acknowledge-flow-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: AcknowledgeFlow
---
