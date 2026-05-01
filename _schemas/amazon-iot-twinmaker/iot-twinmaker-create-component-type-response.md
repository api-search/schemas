---
description: CreateComponentTypeResponse schema
layout: schema
name: CreateComponentTypeResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: creationDateTime
  type: object
- description: ''
  name: state
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-create-component-type-response-schema.json
slug: iot-twinmaker-create-component-type-response
source_filename: iot-twinmaker-create-component-type-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-component-type-response-schema.json\",\n  \"title\": \"CreateComponentTypeResponse\",\n  \"description\": \"CreateComponentTypeResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TwinMakerArn\"\n        },\n        {\n          \"description\": \"The ARN of the component type.\"\n        }\n      ]\n    },\n    \"creationDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the entity was created.\"\n        }\n      ]\n    },\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n   \
  \       \"description\": \"The current state of the component type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"creationDateTime\",\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-component-type-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: CreateComponentTypeResponse
---
