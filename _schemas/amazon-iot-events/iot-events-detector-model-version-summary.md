---
description: Information about the detector model version.
layout: schema
name: DetectorModelVersionSummary
properties_list:
- description: ''
  name: detectorModelName
  type: object
- description: ''
  name: detectorModelVersion
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
  name: evaluationMethod
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-detector-model-version-summary-schema.json
slug: iot-events-detector-model-version-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-version-summary-schema.json\",\n  \"title\": \"DetectorModelVersionSummary\",\n  \"description\": \"Information about the detector model version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelName\"\n        },\n        {\n          \"description\": \"The name of the detector model.\"\n        }\n      ]\n    },\n    \"detectorModelVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelVersion\"\n        },\n        {\n          \"description\": \"The ID of the detector model version.\"\n        }\n      ]\n    },\n    \"detectorModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelArn\"\
  \n        },\n        {\n          \"description\": \"The ARN of the detector model version.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the role that grants the detector model permission to perform its tasks.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the detector model version was created.\"\n        }\n      ]\n    },\n    \"lastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The last time the detector model version was updated.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelVersionStatus\"\
  \n        },\n        {\n          \"description\": \"The status of the detector model version.\"\n        }\n      ]\n    },\n    \"evaluationMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMethod\"\n        },\n        {\n          \"description\": \"Information about the order in which events are evaluated and how actions are executed. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-version-summary-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: DetectorModelVersionSummary
---
