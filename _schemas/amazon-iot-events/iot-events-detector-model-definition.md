---
description: Information that defines how a detector operates.
layout: schema
name: DetectorModelDefinition
properties_list:
- description: ''
  name: states
  type: object
- description: ''
  name: initialStateName
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-detector-model-definition-schema.json
slug: iot-events-detector-model-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-definition-schema.json\",\n  \"title\": \"DetectorModelDefinition\",\n  \"description\": \"Information that defines how a detector operates.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"states\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/States\"\n        },\n        {\n          \"description\": \"Information about the states of the detector.\"\n        }\n      ]\n    },\n    \"initialStateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateName\"\n        },\n        {\n          \"description\": \"The state that is entered at the creation of each detector (instance).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"states\",\n    \"initialStateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-definition-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: DetectorModelDefinition
---
