---
description: StartDetectorModelAnalysisRequest schema
layout: schema
name: StartDetectorModelAnalysisRequest
properties_list:
- description: Information that defines how a detector operates.
  name: detectorModelDefinition
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-start-detector-model-analysis-request-schema.json
slug: iot-events-start-detector-model-analysis-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-start-detector-model-analysis-request-schema.json\",\n  \"title\": \"StartDetectorModelAnalysisRequest\",\n  \"description\": \"StartDetectorModelAnalysisRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModelDefinition\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"states\",\n        \"initialStateName\"\n      ],\n      \"properties\": {\n        \"states\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/States\"\n            },\n            {\n              \"description\": \"Information about the states of the detector.\"\n            }\n          ]\n        },\n        \"initialStateName\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/StateName\"\n  \
  \          },\n            {\n              \"description\": \"The state that is entered at the creation of each detector (instance).\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Information that defines how a detector operates.\"\n    }\n  },\n  \"required\": [\n    \"detectorModelDefinition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-start-detector-model-analysis-request-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: StartDetectorModelAnalysisRequest
---
