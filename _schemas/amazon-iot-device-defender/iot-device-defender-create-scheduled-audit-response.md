---
description: CreateScheduledAuditResponse schema
layout: schema
name: CreateScheduledAuditResponse
properties_list:
- description: ''
  name: scheduledAuditArn
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-create-scheduled-audit-response-schema.json
slug: iot-device-defender-create-scheduled-audit-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-scheduled-audit-response-schema.json\",\n  \"title\": \"CreateScheduledAuditResponse\",\n  \"description\": \"CreateScheduledAuditResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scheduledAuditArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduledAuditArn\"\n        },\n        {\n          \"description\": \"The ARN of the scheduled audit.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-scheduled-audit-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: CreateScheduledAuditResponse
---
