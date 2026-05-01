---
description: UpdateDetectorModelRequest schema
layout: schema
name: UpdateDetectorModelRequest
properties_list:
- description: ''
  name: detectorModelDefinition
  type: object
- description: ''
  name: detectorModelDescription
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: evaluationMethod
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-update-detector-model-request-schema.json
slug: iot-events-update-detector-model-request
source_filename: iot-events-update-detector-model-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-update-detector-model-request-schema.json\",\n  \"title\": \"UpdateDetectorModelRequest\",\n  \"description\": \"UpdateDetectorModelRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModelDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelDefinition\"\n        },\n        {\n          \"description\": \"Information that defines how a detector operates.\"\n        }\n      ]\n    },\n    \"detectorModelDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelDescription\"\n        },\n        {\n          \"description\": \"A brief description of the detector model.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the role that grants permission to AWS IoT Events to perform its operations.\"\n        }\n      ]\n    },\n    \"evaluationMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMethod\"\n        },\n        {\n          \"description\": \"Information about the order in which events are evaluated and how actions are executed. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"detectorModelDefinition\",\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-update-detector-model-request-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: UpdateDetectorModelRequest
---
