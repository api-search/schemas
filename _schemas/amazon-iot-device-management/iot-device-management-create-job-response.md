---
description: CreateJobResponse schema
layout: schema
name: CreateJobResponse
properties_list:
- description: ''
  name: jobArn
  type: object
- description: ''
  name: jobId
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-job-response-schema.json
slug: iot-device-management-create-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-job-response-schema.json\",\n  \"title\": \"CreateJobResponse\",\n  \"description\": \"CreateJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobArn\"\n        },\n        {\n          \"description\": \"The job ARN.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The unique identifier you assigned to this job.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDescription\"\n        },\n        {\n          \"description\": \"The job description.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-job-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateJobResponse
---
