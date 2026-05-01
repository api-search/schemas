---
description: Specifies the default alarm state. The configuration applies to all alarms that were created based on this alarm model.
layout: schema
name: InitializationConfiguration
properties_list:
- description: ''
  name: disabledOnInitialization
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-initialization-configuration-schema.json
slug: iot-events-initialization-configuration
source_filename: iot-events-initialization-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-initialization-configuration-schema.json\",\n  \"title\": \"InitializationConfiguration\",\n  \"description\": \"Specifies the default alarm state. The configuration applies to all alarms that were created based on this alarm model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabledOnInitialization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisabledOnInitialization\"\n        },\n        {\n          \"description\": \"The value must be <code>TRUE</code> or <code>FALSE</code>. If <code>FALSE</code>, all alarm instances created based on the alarm model are activated. The default value is <code>TRUE</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"disabledOnInitialization\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-initialization-configuration-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: InitializationConfiguration
---
