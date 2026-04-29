---
description: Information about the input.
layout: schema
name: InputSummary
properties_list:
- description: ''
  name: inputName
  type: object
- description: ''
  name: inputDescription
  type: object
- description: ''
  name: inputArn
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
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-input-summary-schema.json
slug: iot-events-input-summary
source_filename: iot-events-input-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-input-summary-schema.json\",\n  \"title\": \"InputSummary\",\n  \"description\": \"Information about the input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputName\"\n        },\n        {\n          \"description\": \"The name of the input.\"\n        }\n      ]\n    },\n    \"inputDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDescription\"\n        },\n        {\n          \"description\": \"A brief description of the input.\"\n        }\n      ]\n    },\n    \"inputArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputArn\"\n        },\n        {\n          \"description\": \"The ARN of the input.\"\n\
  \        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the input was created.\"\n        }\n      ]\n    },\n    \"lastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The last time the input was updated.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputStatus\"\n        },\n        {\n          \"description\": \"The status of the input.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-input-summary-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: InputSummary
---
