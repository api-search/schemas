---
description: GetPercentilesResponse schema
layout: schema
name: GetPercentilesResponse
properties_list:
- description: ''
  name: percentiles
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-get-percentiles-response-schema.json
slug: iot-core-get-percentiles-response
source_filename: iot-core-get-percentiles-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-percentiles-response-schema.json\",\n  \"title\": \"GetPercentilesResponse\",\n  \"description\": \"GetPercentilesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"percentiles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentiles\"\n        },\n        {\n          \"description\": \"The percentile values of the aggregated fields.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-percentiles-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: GetPercentilesResponse
---
