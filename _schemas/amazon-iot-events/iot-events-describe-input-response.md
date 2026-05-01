---
description: DescribeInputResponse schema
layout: schema
name: DescribeInputResponse
properties_list:
- description: ''
  name: input
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-describe-input-response-schema.json
slug: iot-events-describe-input-response
source_filename: iot-events-describe-input-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-describe-input-response-schema.json\",\n  \"title\": \"DescribeInputResponse\",\n  \"description\": \"DescribeInputResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Input\"\n        },\n        {\n          \"description\": \"Information about the input.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-describe-input-response-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: DescribeInputResponse
---
