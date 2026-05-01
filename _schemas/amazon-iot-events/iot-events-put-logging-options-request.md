---
description: PutLoggingOptionsRequest schema
layout: schema
name: PutLoggingOptionsRequest
properties_list:
- description: ''
  name: loggingOptions
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-put-logging-options-request-schema.json
slug: iot-events-put-logging-options-request
source_filename: iot-events-put-logging-options-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-put-logging-options-request-schema.json\",\n  \"title\": \"PutLoggingOptionsRequest\",\n  \"description\": \"PutLoggingOptionsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"loggingOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingOptions\"\n        },\n        {\n          \"description\": \"The new values of the AWS IoT Events logging options.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"loggingOptions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-put-logging-options-request-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: PutLoggingOptionsRequest
---
