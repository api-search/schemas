---
description: UpdateEntityResponse schema
layout: schema
name: UpdateEntityResponse
properties_list:
- description: ''
  name: updateDateTime
  type: object
- description: ''
  name: state
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-update-entity-response-schema.json
slug: iot-twinmaker-update-entity-response
source_filename: iot-twinmaker-update-entity-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-entity-response-schema.json\",\n  \"title\": \"UpdateEntityResponse\",\n  \"description\": \"UpdateEntityResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the entity was last updated.\"\n        }\n      ]\n    },\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"The current state of the entity update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"updateDateTime\",\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-entity-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: UpdateEntityResponse
---
