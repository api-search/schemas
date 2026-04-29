---
description: AggregationTypeValues schema
layout: schema
name: AggregationTypeValues
properties_list: []
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-aggregation-type-values-schema.json
slug: iot-core-aggregation-type-values
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-aggregation-type-values-schema.json\",\n  \"title\": \"AggregationTypeValues\",\n  \"description\": \"AggregationTypeValues schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"[a-zA-Z0-9]+\",\n    \"minLength\": 1,\n    \"maxLength\": 12\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-aggregation-type-values-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: AggregationTypeValues
---
