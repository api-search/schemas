---
description: ErrorEntries schema
layout: schema
name: ErrorEntries
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-error-entries-schema.json
slug: iot-twinmaker-error-entries
source_filename: iot-twinmaker-error-entries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-error-entries-schema.json\",\n  \"title\": \"ErrorEntries\",\n  \"description\": \"ErrorEntries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"errors\"\n    ],\n    \"properties\": {\n      \"errors\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Errors\"\n          },\n          {\n            \"description\": \"A list of objects that contain information about errors returned by the <code>BatchPutProperty</code> action.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that contains information about errors returned by the <code>BatchPutProperty</code> action.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-error-entries-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ErrorEntries
---
