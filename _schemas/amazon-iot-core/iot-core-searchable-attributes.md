---
description: SearchableAttributes schema
layout: schema
name: SearchableAttributes
properties_list: []
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-searchable-attributes-schema.json
slug: iot-core-searchable-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-searchable-attributes-schema.json\",\n  \"title\": \"SearchableAttributes\",\n  \"description\": \"SearchableAttributes schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"[a-zA-Z0-9_.,@/:#-]+\",\n    \"maxLength\": 128\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-searchable-attributes-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: SearchableAttributes
---
