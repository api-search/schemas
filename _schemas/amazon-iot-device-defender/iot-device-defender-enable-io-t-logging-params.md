---
description: Parameters used when defining a mitigation action that enable Amazon Web Services IoT Core logging.
layout: schema
name: EnableIoTLoggingParams
properties_list:
- description: ''
  name: roleArnForLogging
  type: object
- description: ''
  name: logLevel
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-enable-io-t-logging-params-schema.json
slug: iot-device-defender-enable-io-t-logging-params
source_filename: iot-device-defender-enable-io-t-logging-params-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-enable-io-t-logging-params-schema.json\",\n  \"title\": \"EnableIoTLoggingParams\",\n  \"description\": \"Parameters used when defining a mitigation action that enable Amazon Web Services IoT Core logging.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleArnForLogging\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role used for logging.\"\n        }\n      ]\n    },\n    \"logLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"Specifies the type of information to be logged.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"roleArnForLogging\",\n    \"logLevel\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-enable-io-t-logging-params-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: EnableIoTLoggingParams
---
