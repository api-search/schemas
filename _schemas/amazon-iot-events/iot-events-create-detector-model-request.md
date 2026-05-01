---
description: CreateDetectorModelRequest schema
layout: schema
name: CreateDetectorModelRequest
properties_list:
- description: ''
  name: detectorModelName
  type: object
- description: ''
  name: detectorModelDefinition
  type: object
- description: ''
  name: detectorModelDescription
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: evaluationMethod
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-create-detector-model-request-schema.json
slug: iot-events-create-detector-model-request
source_filename: iot-events-create-detector-model-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-create-detector-model-request-schema.json\",\n  \"title\": \"CreateDetectorModelRequest\",\n  \"description\": \"CreateDetectorModelRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelName\"\n        },\n        {\n          \"description\": \"The name of the detector model.\"\n        }\n      ]\n    },\n    \"detectorModelDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelDefinition\"\n        },\n        {\n          \"description\": \"Information that defines how the detectors operate.\"\n        }\n      ]\n    },\n    \"detectorModelDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/DetectorModelDescription\"\n        },\n        {\n          \"description\": \"A brief description of the detector model.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeJsonPath\"\n        },\n        {\n          \"description\": \"The input attribute key used to identify a device or system to create a detector (an instance of the detector model) and then to route each input received to the appropriate detector (instance). This parameter uses a JSON-path expression in the message payload of each input to specify the attribute-value pair that is used to identify the device associated with the input.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the role that grants permission to AWS IoT Events to perform its operations.\"\
  \n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"Metadata that can be used to manage the detector model.\"\n        }\n      ]\n    },\n    \"evaluationMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMethod\"\n        },\n        {\n          \"description\": \"Information about the order in which events are evaluated and how actions are executed. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"detectorModelName\",\n    \"detectorModelDefinition\",\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-create-detector-model-request-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: CreateDetectorModelRequest
---
