---
description: GetOTAUpdateResponse schema
layout: schema
name: GetOTAUpdateResponse
properties_list:
- description: ''
  name: otaUpdateInfo
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-get-o-t-a-update-response-schema.json
slug: iot-device-management-get-o-t-a-update-response
source_filename: iot-device-management-get-o-t-a-update-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-o-t-a-update-response-schema.json\",\n  \"title\": \"GetOTAUpdateResponse\",\n  \"description\": \"GetOTAUpdateResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"otaUpdateInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OTAUpdateInfo\"\n        },\n        {\n          \"description\": \"The OTA update info.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-o-t-a-update-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: GetOTAUpdateResponse
---
