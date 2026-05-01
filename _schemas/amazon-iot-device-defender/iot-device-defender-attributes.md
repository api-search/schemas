---
description: Attributes schema
layout: schema
name: Attributes
properties_list: []
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-attributes-schema.json
slug: iot-device-defender-attributes
source_filename: iot-device-defender-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-attributes-schema.json\",\n  \"title\": \"Attributes\",\n  \"description\": \"Attributes schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"string\",\n    \"pattern\": \"[a-zA-Z0-9_.,@/:#-]*\",\n    \"maxLength\": 800\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-attributes-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: Attributes
---
