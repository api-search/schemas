---
description: Errors schema
layout: schema
name: Errors
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-errors-schema.json
slug: iot-twinmaker-errors
source_filename: iot-twinmaker-errors-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-errors-schema.json\",\n  \"title\": \"Errors\",\n  \"description\": \"Errors schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"errorCode\",\n      \"errorMessage\",\n      \"entry\"\n    ],\n    \"properties\": {\n      \"errorCode\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"The error code.\"\n          }\n        ]\n      },\n      \"errorMessage\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"The error message.\"\n          }\n        ]\n      },\n      \"entry\": {\n        \"allOf\": [\n          {\n           \
  \ \"$ref\": \"#/components/schemas/PropertyValueEntry\"\n          },\n          {\n            \"description\": \"An object that contains information about errors returned by the <code>BatchPutProperty</code> action.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An error returned by the <code>BatchPutProperty</code> action.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-errors-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: Errors
---
