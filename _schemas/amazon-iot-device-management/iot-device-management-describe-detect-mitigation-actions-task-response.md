---
description: DescribeDetectMitigationActionsTaskResponse schema
layout: schema
name: DescribeDetectMitigationActionsTaskResponse
properties_list:
- description: ''
  name: taskSummary
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-detect-mitigation-actions-task-response-schema.json
slug: iot-device-management-describe-detect-mitigation-actions-task-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-detect-mitigation-actions-task-response-schema.json\",\n  \"title\": \"DescribeDetectMitigationActionsTaskResponse\",\n  \"description\": \"DescribeDetectMitigationActionsTaskResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectMitigationActionsTaskSummary\"\n        },\n        {\n          \"description\": \" The description of a task. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-detect-mitigation-actions-task-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeDetectMitigationActionsTaskResponse
---
