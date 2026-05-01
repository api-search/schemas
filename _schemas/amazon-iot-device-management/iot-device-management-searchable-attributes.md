---
description: SearchableAttributes schema
layout: schema
name: SearchableAttributes
properties_list: []
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-searchable-attributes-schema.json
slug: iot-device-management-searchable-attributes
source_filename: iot-device-management-searchable-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-searchable-attributes-schema.json\",\n  \"title\": \"SearchableAttributes\",\n  \"description\": \"SearchableAttributes schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"[a-zA-Z0-9_.,@/:#-]+\",\n    \"maxLength\": 128\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-searchable-attributes-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: SearchableAttributes
---
