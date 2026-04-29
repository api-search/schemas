---
description: Attributes schema
layout: schema
name: Attributes
properties_list: []
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-attributes-schema.json
slug: iot-device-management-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-attributes-schema.json\",\n  \"title\": \"Attributes\",\n  \"description\": \"Attributes schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"string\",\n    \"pattern\": \"[a-zA-Z0-9_.,@/:#-]*\",\n    \"maxLength\": 800\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-attributes-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: Attributes
---
