---
description: DescribeDetectMitigationActionsTaskResponse schema
layout: schema
name: DescribeDetectMitigationActionsTaskResponse
properties_list:
- description: ''
  name: taskSummary
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-describe-detect-mitigation-actions-task-response-schema.json
slug: iot-core-describe-detect-mitigation-actions-task-response
source_filename: iot-core-describe-detect-mitigation-actions-task-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-detect-mitigation-actions-task-response-schema.json\",\n  \"title\": \"DescribeDetectMitigationActionsTaskResponse\",\n  \"description\": \"DescribeDetectMitigationActionsTaskResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectMitigationActionsTaskSummary\"\n        },\n        {\n          \"description\": \" The description of a task. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-detect-mitigation-actions-task-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: DescribeDetectMitigationActionsTaskResponse
---
