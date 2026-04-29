---
description: DescribeLoggingOptionsResponse schema
layout: schema
name: DescribeLoggingOptionsResponse
properties_list:
- description: ''
  name: loggingOptions
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-describe-logging-options-response-schema.json
slug: iot-events-describe-logging-options-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-describe-logging-options-response-schema.json\",\n  \"title\": \"DescribeLoggingOptionsResponse\",\n  \"description\": \"DescribeLoggingOptionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"loggingOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingOptions\"\n        },\n        {\n          \"description\": \"The current settings of the AWS IoT Events logging options.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-describe-logging-options-response-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: DescribeLoggingOptionsResponse
---
