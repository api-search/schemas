---
description: ListAuditMitigationActionsTasksResponse schema
layout: schema
name: ListAuditMitigationActionsTasksResponse
properties_list:
- description: ''
  name: tasks
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-audit-mitigation-actions-tasks-response-schema.json
slug: iot-core-list-audit-mitigation-actions-tasks-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-audit-mitigation-actions-tasks-response-schema.json\",\n  \"title\": \"ListAuditMitigationActionsTasksResponse\",\n  \"description\": \"ListAuditMitigationActionsTasksResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tasks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditMitigationActionsTaskMetadataList\"\n        },\n        {\n          \"description\": \"The collection of audit mitigation tasks that matched the filter criteria.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-audit-mitigation-actions-tasks-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListAuditMitigationActionsTasksResponse
---
