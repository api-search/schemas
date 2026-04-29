---
description: OrderByList schema
layout: schema
name: OrderByList
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-order-by-list-schema.json
slug: iot-twinmaker-order-by-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-order-by-list-schema.json\",\n  \"title\": \"OrderByList\",\n  \"description\": \"OrderByList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"propertyName\"\n    ],\n    \"properties\": {\n      \"order\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Order\"\n          },\n          {\n            \"description\": \"The set order that filters results.\"\n          }\n        ]\n      },\n      \"propertyName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"The property name.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Filter criteria that orders the return output.\
  \ It can be sorted in ascending or descending order.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-order-by-list-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: OrderByList
---
