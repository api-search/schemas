---
description: The scene error.
layout: schema
name: SceneError
properties_list:
- description: ''
  name: code
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-scene-error-schema.json
slug: iot-twinmaker-scene-error
source_filename: iot-twinmaker-scene-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-scene-error-schema.json\",\n  \"title\": \"SceneError\",\n  \"description\": \"The scene error.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SceneErrorCode\"\n        },\n        {\n          \"description\": \"The SceneError code.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \"The SceneError message.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-scene-error-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: SceneError
---
