---
description: DescribeAuditMitigationActionsTaskResponse schema
layout: schema
name: DescribeAuditMitigationActionsTaskResponse
properties_list:
- description: ''
  name: taskStatus
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: taskStatistics
  type: object
- description: ''
  name: target
  type: object
- description: ''
  name: auditCheckToActionsMapping
  type: object
- description: ''
  name: actionsDefinition
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-audit-mitigation-actions-task-response-schema.json
slug: iot-device-defender-describe-audit-mitigation-actions-task-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-audit-mitigation-actions-task-response-schema.json\",\n  \"title\": \"DescribeAuditMitigationActionsTaskResponse\",\n  \"description\": \"DescribeAuditMitigationActionsTaskResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditMitigationActionsTaskStatus\"\n        },\n        {\n          \"description\": \"The current status of the task.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the task was started.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the task was completed or canceled.\"\n        }\n      ]\n    },\n    \"taskStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditMitigationActionsTaskStatistics\"\n        },\n        {\n          \"description\": \"Aggregate counts of the results when the mitigation tasks were applied to the findings for this audit mitigation actions task.\"\n        }\n      ]\n    },\n    \"target\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditMitigationActionsTaskTarget\"\n        },\n        {\n          \"description\": \"Identifies the findings to which the mitigation actions are applied. This can be by audit checks, by audit task, or a set of findings.\"\n        }\n      ]\n    },\n    \"auditCheckToActionsMapping\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditCheckToActionsMapping\"\
  \n        },\n        {\n          \"description\": \"Specifies the mitigation actions that should be applied to specific audit checks.\"\n        }\n      ]\n    },\n    \"actionsDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionList\"\n        },\n        {\n          \"description\": \"Specifies the mitigation actions and their parameters that are applied as part of this task.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-audit-mitigation-actions-task-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeAuditMitigationActionsTaskResponse
---
