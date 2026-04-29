---
description: ListDetectMitigationActionsTasksResponse schema
layout: schema
name: ListDetectMitigationActionsTasksResponse
properties_list:
- description: ''
  name: tasks
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-detect-mitigation-actions-tasks-response-schema.json
slug: iot-device-management-list-detect-mitigation-actions-tasks-response
source_filename: iot-device-management-list-detect-mitigation-actions-tasks-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-detect-mitigation-actions-tasks-response-schema.json\",\n  \"title\": \"ListDetectMitigationActionsTasksResponse\",\n  \"description\": \"ListDetectMitigationActionsTasksResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tasks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectMitigationActionsTaskSummaryList\"\n        },\n        {\n          \"description\": \" The collection of ML Detect mitigation tasks that matched the filter criteria. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" A token that can be used to retrieve the next set of results, or <code>null</code>\
  \ if there are no additional results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-detect-mitigation-actions-tasks-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListDetectMitigationActionsTasksResponse
---
