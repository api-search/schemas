---
description: Information about how the detector model is configured.
layout: schema
name: DetectorModelConfiguration
properties_list:
- description: ''
  name: detectorModelName
  type: object
- description: ''
  name: detectorModelVersion
  type: object
- description: ''
  name: detectorModelDescription
  type: object
- description: ''
  name: detectorModelArn
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: lastUpdateTime
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: evaluationMethod
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-detector-model-configuration-schema.json
slug: iot-events-detector-model-configuration
source_filename: iot-events-detector-model-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-configuration-schema.json\",\n  \"title\": \"DetectorModelConfiguration\",\n  \"description\": \"Information about how the detector model is configured.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelName\"\n        },\n        {\n          \"description\": \"The name of the detector model.\"\n        }\n      ]\n    },\n    \"detectorModelVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelVersion\"\n        },\n        {\n          \"description\": \"The version of the detector model.\"\n        }\n      ]\n    },\n    \"detectorModelDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelDescription\"\
  \n        },\n        {\n          \"description\": \"A brief description of the detector model.\"\n        }\n      ]\n    },\n    \"detectorModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelArn\"\n        },\n        {\n          \"description\": \"The ARN of the detector model.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the role that grants permission to AWS IoT Events to perform its operations.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the detector model was created.\"\n        }\n      ]\n    },\n    \"lastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The time the detector model was last updated.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelVersionStatus\"\n        },\n        {\n          \"description\": \"The status of the detector model.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeJsonPath\"\n        },\n        {\n          \"description\": \"<p>The value used to identify a detector instance. When a device or system sends input, a new detector instance with a unique key value is created. AWS IoT Events can continue to route input to its corresponding detector instance based on this identifying information. </p> <p>This parameter uses a JSON-path expression to select the attribute-value pair in the message payload that is used for identification. To route the message to the correct detector instance,\
  \ the device must send a message payload that contains the same attribute-value.</p>\"\n        }\n      ]\n    },\n    \"evaluationMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMethod\"\n        },\n        {\n          \"description\": \"Information about the order in which events are evaluated and how actions are executed. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-configuration-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: DetectorModelConfiguration
---
