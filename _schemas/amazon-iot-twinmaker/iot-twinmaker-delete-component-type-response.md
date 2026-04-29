---
description: DeleteComponentTypeResponse schema
layout: schema
name: DeleteComponentTypeResponse
properties_list:
- description: ''
  name: state
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-delete-component-type-response-schema.json
slug: iot-twinmaker-delete-component-type-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-delete-component-type-response-schema.json\",\n  \"title\": \"DeleteComponentTypeResponse\",\n  \"description\": \"DeleteComponentTypeResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"The current state of the component type to be deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-delete-component-type-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: DeleteComponentTypeResponse
---
