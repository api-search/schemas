---
description: DescribeAuditTaskResponse schema
layout: schema
name: DescribeAuditTaskResponse
properties_list:
- description: ''
  name: taskStatus
  type: object
- description: ''
  name: taskType
  type: object
- description: ''
  name: taskStartTime
  type: object
- description: ''
  name: taskStatistics
  type: object
- description: ''
  name: scheduledAuditName
  type: object
- description: ''
  name: auditDetails
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-describe-audit-task-response-schema.json
slug: iot-core-describe-audit-task-response
source_filename: iot-core-describe-audit-task-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-audit-task-response-schema.json\",\n  \"title\": \"DescribeAuditTaskResponse\",\n  \"description\": \"DescribeAuditTaskResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditTaskStatus\"\n        },\n        {\n          \"description\": \"The status of the audit: one of \\\"IN_PROGRESS\\\", \\\"COMPLETED\\\", \\\"FAILED\\\", or \\\"CANCELED\\\".\"\n        }\n      ]\n    },\n    \"taskType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditTaskType\"\n        },\n        {\n          \"description\": \"The type of audit: \\\"ON_DEMAND_AUDIT_TASK\\\" or \\\"SCHEDULED_AUDIT_TASK\\\".\"\n        }\n      ]\n    },\n    \"taskStartTime\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the audit started.\"\n        }\n      ]\n    },\n    \"taskStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStatistics\"\n        },\n        {\n          \"description\": \"Statistical information about the audit.\"\n        }\n      ]\n    },\n    \"scheduledAuditName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduledAuditName\"\n        },\n        {\n          \"description\": \"The name of the scheduled audit (only if the audit was a scheduled audit).\"\n        }\n      ]\n    },\n    \"auditDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditDetails\"\n        },\n        {\n          \"description\": \"Detailed information about each check performed during this audit.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-audit-task-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: DescribeAuditTaskResponse
---
