---
description: GetCardinalityResponse schema
layout: schema
name: GetCardinalityResponse
properties_list:
- description: ''
  name: cardinality
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-get-cardinality-response-schema.json
slug: iot-device-defender-get-cardinality-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-get-cardinality-response-schema.json\",\n  \"title\": \"GetCardinalityResponse\",\n  \"description\": \"GetCardinalityResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardinality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The approximate count of unique values that match the query.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-get-cardinality-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: GetCardinalityResponse
---
