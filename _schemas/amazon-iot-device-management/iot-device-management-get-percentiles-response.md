---
description: GetPercentilesResponse schema
layout: schema
name: GetPercentilesResponse
properties_list:
- description: ''
  name: percentiles
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-get-percentiles-response-schema.json
slug: iot-device-management-get-percentiles-response
source_filename: iot-device-management-get-percentiles-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-percentiles-response-schema.json\",\n  \"title\": \"GetPercentilesResponse\",\n  \"description\": \"GetPercentilesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"percentiles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentiles\"\n        },\n        {\n          \"description\": \"The percentile values of the aggregated fields.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-percentiles-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: GetPercentilesResponse
---
