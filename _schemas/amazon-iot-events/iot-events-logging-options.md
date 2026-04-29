---
description: The values of the AWS IoT Events logging options.
layout: schema
name: LoggingOptions
properties_list:
- description: ''
  name: roleArn
  type: object
- description: ''
  name: level
  type: object
- description: ''
  name: enabled
  type: object
- description: ''
  name: detectorDebugOptions
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-logging-options-schema.json
slug: iot-events-logging-options
source_filename: iot-events-logging-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-logging-options-schema.json\",\n  \"title\": \"LoggingOptions\",\n  \"description\": \"The values of the AWS IoT Events logging options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the role that grants permission to AWS IoT Events to perform logging.\"\n        }\n      ]\n    },\n    \"level\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingLevel\"\n        },\n        {\n          \"description\": \"The logging level.\"\n        }\n      ]\n    },\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingEnabled\"\n        },\n\
  \        {\n          \"description\": \"If TRUE, logging is enabled for AWS IoT Events.\"\n        }\n      ]\n    },\n    \"detectorDebugOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorDebugOptions\"\n        },\n        {\n          \"description\": \"Information that identifies those detector models and their detectors (instances) for which the logging level is given.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"roleArn\",\n    \"level\",\n    \"enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-logging-options-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: LoggingOptions
---
