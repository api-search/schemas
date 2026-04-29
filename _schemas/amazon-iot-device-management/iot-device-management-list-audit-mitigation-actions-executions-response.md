---
description: ListAuditMitigationActionsExecutionsResponse schema
layout: schema
name: ListAuditMitigationActionsExecutionsResponse
properties_list:
- description: ''
  name: actionsExecutions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-audit-mitigation-actions-executions-response-schema.json
slug: iot-device-management-list-audit-mitigation-actions-executions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-audit-mitigation-actions-executions-response-schema.json\",\n  \"title\": \"ListAuditMitigationActionsExecutionsResponse\",\n  \"description\": \"ListAuditMitigationActionsExecutionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionsExecutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditMitigationActionExecutionMetadataList\"\n        },\n        {\n          \"description\": \"A set of task execution results based on the input parameters. Details include the mitigation action applied, start time, and task status.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\"\
  : \"The token for the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-audit-mitigation-actions-executions-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListAuditMitigationActionsExecutionsResponse
---
