---
description: DetectorDebugOptions schema
layout: schema
name: DetectorDebugOptions
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-detector-debug-options-schema.json
slug: iot-events-detector-debug-options
source_filename: iot-events-detector-debug-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-debug-options-schema.json\",\n  \"title\": \"DetectorDebugOptions\",\n  \"description\": \"DetectorDebugOptions schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"detectorModelName\"\n    ],\n    \"properties\": {\n      \"detectorModelName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DetectorModelName\"\n          },\n          {\n            \"description\": \"The name of the detector model.\"\n          }\n        ]\n      },\n      \"keyValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/KeyValue\"\n          },\n          {\n            \"description\": \"The value of the input attribute key used to create the detector (the instance of the detector\
  \ model).\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The detector model and the specific detectors (instances) for which the logging level is given.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-debug-options-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: DetectorDebugOptions
---
