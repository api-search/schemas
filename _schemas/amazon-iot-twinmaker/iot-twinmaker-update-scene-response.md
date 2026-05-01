---
description: UpdateSceneResponse schema
layout: schema
name: UpdateSceneResponse
properties_list:
- description: ''
  name: updateDateTime
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-update-scene-response-schema.json
slug: iot-twinmaker-update-scene-response
source_filename: iot-twinmaker-update-scene-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-scene-response-schema.json\",\n  \"title\": \"UpdateSceneResponse\",\n  \"description\": \"UpdateSceneResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the scene was last updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"updateDateTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-scene-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: UpdateSceneResponse
---
