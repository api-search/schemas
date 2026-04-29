---
description: CreateScheduledAuditResponse schema
layout: schema
name: CreateScheduledAuditResponse
properties_list:
- description: ''
  name: scheduledAuditArn
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-scheduled-audit-response-schema.json
slug: iot-device-management-create-scheduled-audit-response
source_filename: iot-device-management-create-scheduled-audit-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-scheduled-audit-response-schema.json\",\n  \"title\": \"CreateScheduledAuditResponse\",\n  \"description\": \"CreateScheduledAuditResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scheduledAuditArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduledAuditArn\"\n        },\n        {\n          \"description\": \"The ARN of the scheduled audit.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-scheduled-audit-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateScheduledAuditResponse
---
