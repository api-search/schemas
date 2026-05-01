---
description: Filter criteria that orders the return output. It can be sorted in ascending or descending order.
layout: schema
name: OrderBy
properties_list:
- description: ''
  name: order
  type: object
- description: ''
  name: propertyName
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-order-by-schema.json
slug: iot-twinmaker-order-by
source_filename: iot-twinmaker-order-by-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-order-by-schema.json\",\n  \"title\": \"OrderBy\",\n  \"description\": \"Filter criteria that orders the return output. It can be sorted in ascending or descending order.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"order\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Order\"\n        },\n        {\n          \"description\": \"The set order that filters results.\"\n        }\n      ]\n    },\n    \"propertyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The property name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"propertyName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-order-by-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: OrderBy
---
