---
description: DescribeJobExecutionResponse schema
layout: schema
name: DescribeJobExecutionResponse
properties_list:
- description: ''
  name: execution
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-job-execution-response-schema.json
slug: iot-device-defender-describe-job-execution-response
source_filename: iot-device-defender-describe-job-execution-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-job-execution-response-schema.json\",\n  \"title\": \"DescribeJobExecutionResponse\",\n  \"description\": \"DescribeJobExecutionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"execution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobExecution\"\n        },\n        {\n          \"description\": \"Information about the job execution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-job-execution-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeJobExecutionResponse
---
