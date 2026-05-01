---
description: UpdateDetectorModelResponse schema
layout: schema
name: UpdateDetectorModelResponse
properties_list:
- description: ''
  name: detectorModelConfiguration
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-update-detector-model-response-schema.json
slug: iot-events-update-detector-model-response
source_filename: iot-events-update-detector-model-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-update-detector-model-response-schema.json\",\n  \"title\": \"UpdateDetectorModelResponse\",\n  \"description\": \"UpdateDetectorModelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModelConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelConfiguration\"\n        },\n        {\n          \"description\": \"Information about how the detector model is configured.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-update-detector-model-response-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: UpdateDetectorModelResponse
---
