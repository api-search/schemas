---
description: ListAuditSuppressionsResponse schema
layout: schema
name: ListAuditSuppressionsResponse
properties_list:
- description: ''
  name: suppressions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-audit-suppressions-response-schema.json
slug: iot-device-defender-list-audit-suppressions-response
source_filename: iot-device-defender-list-audit-suppressions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-audit-suppressions-response-schema.json\",\n  \"title\": \"ListAuditSuppressionsResponse\",\n  \"description\": \"ListAuditSuppressionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"suppressions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditSuppressionList\"\n        },\n        {\n          \"description\": \" List of audit suppressions. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" A token that can be used to retrieve the next set of results, or <code>null</code> if there are no additional results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-audit-suppressions-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListAuditSuppressionsResponse
---
