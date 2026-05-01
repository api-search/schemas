---
description: CreateJobTemplateResponse schema
layout: schema
name: CreateJobTemplateResponse
properties_list:
- description: ''
  name: jobTemplateArn
  type: object
- description: ''
  name: jobTemplateId
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-job-template-response-schema.json
slug: iot-device-management-create-job-template-response
source_filename: iot-device-management-create-job-template-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-job-template-response-schema.json\",\n  \"title\": \"CreateJobTemplateResponse\",\n  \"description\": \"CreateJobTemplateResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobTemplateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTemplateArn\"\n        },\n        {\n          \"description\": \"The ARN of the job template.\"\n        }\n      ]\n    },\n    \"jobTemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTemplateId\"\n        },\n        {\n          \"description\": \"The unique identifier of the job template.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-job-template-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateJobTemplateResponse
---
