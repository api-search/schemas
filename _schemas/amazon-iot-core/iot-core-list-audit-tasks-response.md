---
description: ListAuditTasksResponse schema
layout: schema
name: ListAuditTasksResponse
properties_list:
- description: ''
  name: tasks
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-audit-tasks-response-schema.json
slug: iot-core-list-audit-tasks-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-audit-tasks-response-schema.json\",\n  \"title\": \"ListAuditTasksResponse\",\n  \"description\": \"ListAuditTasksResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tasks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditTaskMetadataList\"\n        },\n        {\n          \"description\": \"The audits that were performed during the specified time period.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that can be used to retrieve the next set of results, or <code>null</code> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-audit-tasks-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListAuditTasksResponse
---
