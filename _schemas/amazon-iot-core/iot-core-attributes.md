---
description: Attributes schema
layout: schema
name: Attributes
properties_list: []
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-attributes-schema.json
slug: iot-core-attributes
source_filename: iot-core-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-attributes-schema.json\",\n  \"title\": \"Attributes\",\n  \"description\": \"Attributes schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"string\",\n    \"pattern\": \"[a-zA-Z0-9_.,@/:#-]*\",\n    \"maxLength\": 800\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-attributes-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: Attributes
---
