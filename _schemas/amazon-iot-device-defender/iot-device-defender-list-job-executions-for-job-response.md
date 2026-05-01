---
description: ListJobExecutionsForJobResponse schema
layout: schema
name: ListJobExecutionsForJobResponse
properties_list:
- description: ''
  name: executionSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-job-executions-for-job-response-schema.json
slug: iot-device-defender-list-job-executions-for-job-response
source_filename: iot-device-defender-list-job-executions-for-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-job-executions-for-job-response-schema.json\",\n  \"title\": \"ListJobExecutionsForJobResponse\",\n  \"description\": \"ListJobExecutionsForJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executionSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobExecutionSummaryForJobList\"\n        },\n        {\n          \"description\": \"A list of job execution summaries.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or <b>null</b> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-job-executions-for-job-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListJobExecutionsForJobResponse
---
