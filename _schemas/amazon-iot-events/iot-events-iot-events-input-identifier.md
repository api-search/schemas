---
description: The identifier of the input routed to AWS IoT Events.
layout: schema
name: IotEventsInputIdentifier
properties_list:
- description: ''
  name: inputName
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-iot-events-input-identifier-schema.json
slug: iot-events-iot-events-input-identifier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-events-input-identifier-schema.json\",\n  \"title\": \"IotEventsInputIdentifier\",\n  \"description\": \" The identifier of the input routed to AWS IoT Events. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputName\"\n        },\n        {\n          \"description\": \" The name of the input routed to AWS IoT Events. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-events-input-identifier-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: IotEventsInputIdentifier
---
