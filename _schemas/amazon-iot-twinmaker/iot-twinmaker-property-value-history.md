---
description: The history of values for a time series property.
layout: schema
name: PropertyValueHistory
properties_list:
- description: ''
  name: entityPropertyReference
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-value-history-schema.json
slug: iot-twinmaker-property-value-history
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-value-history-schema.json\",\n  \"title\": \"PropertyValueHistory\",\n  \"description\": \"The history of values for a time series property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityPropertyReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityPropertyReference\"\n        },\n        {\n          \"description\": \"An object that uniquely identifies an entity property.\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Values\"\n        },\n        {\n          \"description\": \"A list of objects that contain information about the values in the history of a time series property.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  entityPropertyReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-value-history-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyValueHistory
---
