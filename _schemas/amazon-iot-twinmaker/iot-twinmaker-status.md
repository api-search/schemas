---
description: An object that represents the status of an entity, component, component type, or workspace.
layout: schema
name: Status
properties_list:
- description: ''
  name: state
  type: object
- description: ''
  name: error
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-status-schema.json
slug: iot-twinmaker-status
source_filename: iot-twinmaker-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-status-schema.json\",\n  \"title\": \"Status\",\n  \"description\": \"An object that represents the status of an entity, component, component type, or workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"The current state of the entity, component, component type, or workspace.\"\n        }\n      ]\n    },\n    \"error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorDetails\"\n        },\n        {\n          \"description\": \"The error message.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-status-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: Status
---
