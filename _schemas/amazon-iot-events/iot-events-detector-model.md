---
description: Information about the detector model.
layout: schema
name: DetectorModel
properties_list:
- description: ''
  name: detectorModelDefinition
  type: object
- description: ''
  name: detectorModelConfiguration
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-detector-model-schema.json
slug: iot-events-detector-model
source_filename: iot-events-detector-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-schema.json\",\n  \"title\": \"DetectorModel\",\n  \"description\": \"Information about the detector model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModelDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelDefinition\"\n        },\n        {\n          \"description\": \"Information that defines how a detector operates.\"\n        }\n      ]\n    },\n    \"detectorModelConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelConfiguration\"\n        },\n        {\n          \"description\": \"Information about how the detector is configured.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: DetectorModel
---
