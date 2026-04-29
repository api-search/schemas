---
description: Information about the detector model.
layout: schema
name: DetectorModelSummary
properties_list:
- description: ''
  name: detectorModelName
  type: object
- description: ''
  name: detectorModelDescription
  type: object
- description: ''
  name: creationTime
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-detector-model-summary-schema.json
slug: iot-events-detector-model-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-summary-schema.json\",\n  \"title\": \"DetectorModelSummary\",\n  \"description\": \"Information about the detector model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelName\"\n        },\n        {\n          \"description\": \"The name of the detector model.\"\n        }\n      ]\n    },\n    \"detectorModelDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelDescription\"\n        },\n        {\n          \"description\": \"A brief description of the detector model.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The time the detector model was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-summary-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: DetectorModelSummary
---
