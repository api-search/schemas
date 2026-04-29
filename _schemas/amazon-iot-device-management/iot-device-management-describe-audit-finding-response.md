---
description: DescribeAuditFindingResponse schema
layout: schema
name: DescribeAuditFindingResponse
properties_list:
- description: The findings (results) of the audit.
  name: finding
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-audit-finding-response-schema.json
slug: iot-device-management-describe-audit-finding-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-audit-finding-response-schema.json\",\n  \"title\": \"DescribeAuditFindingResponse\",\n  \"description\": \"DescribeAuditFindingResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"finding\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"findingId\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/FindingId\"\n            },\n            {\n              \"description\": \"A unique identifier for this set of audit findings. This identifier is used to apply mitigation tasks to one or more sets of findings.\"\n            }\n          ]\n        },\n        \"taskId\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/AuditTaskId\"\n         \
  \   },\n            {\n              \"description\": \"The ID of the audit that generated this result (finding).\"\n            }\n          ]\n        },\n        \"checkName\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/AuditCheckName\"\n            },\n            {\n              \"description\": \"The audit check that generated this result.\"\n            }\n          ]\n        },\n        \"taskStartTime\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Timestamp\"\n            },\n            {\n              \"description\": \"The time the audit started.\"\n            }\n          ]\n        },\n        \"findingTime\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Timestamp\"\n            },\n            {\n              \"description\": \"The time the result (finding) was discovered.\"\n            }\n          ]\n        },\n        \"severity\"\
  : {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/AuditFindingSeverity\"\n            },\n            {\n              \"description\": \"The severity of the result (finding).\"\n            }\n          ]\n        },\n        \"nonCompliantResource\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/NonCompliantResource\"\n            },\n            {\n              \"description\": \"The resource that was found to be noncompliant with the audit check.\"\n            }\n          ]\n        },\n        \"relatedResources\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/RelatedResources\"\n            },\n            {\n              \"description\": \"The list of related resources.\"\n            }\n          ]\n        },\n        \"reasonForNonCompliance\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ReasonForNonCompliance\"\
  \n            },\n            {\n              \"description\": \"The reason the resource was noncompliant.\"\n            }\n          ]\n        },\n        \"reasonForNonComplianceCode\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ReasonForNonComplianceCode\"\n            },\n            {\n              \"description\": \"A code that indicates the reason that the resource was noncompliant.\"\n            }\n          ]\n        },\n        \"isSuppressed\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/IsSuppressed\"\n            },\n            {\n              \"description\": \" Indicates whether the audit finding was suppressed or not during reporting. \"\n            }\n          ]\n        }\n      },\n      \"description\": \"The findings (results) of the audit.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-audit-finding-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeAuditFindingResponse
---
