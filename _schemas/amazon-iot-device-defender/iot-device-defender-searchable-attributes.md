---
description: SearchableAttributes schema
layout: schema
name: SearchableAttributes
properties_list: []
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-searchable-attributes-schema.json
slug: iot-device-defender-searchable-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-searchable-attributes-schema.json\",\n  \"title\": \"SearchableAttributes\",\n  \"description\": \"SearchableAttributes schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"[a-zA-Z0-9_.,@/:#-]+\",\n    \"maxLength\": 128\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-searchable-attributes-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: SearchableAttributes
---
