---
description: GetEffectivePoliciesResponse schema
layout: schema
name: GetEffectivePoliciesResponse
properties_list:
- description: ''
  name: effectivePolicies
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-get-effective-policies-response-schema.json
slug: iot-core-get-effective-policies-response
source_filename: iot-core-get-effective-policies-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-effective-policies-response-schema.json\",\n  \"title\": \"GetEffectivePoliciesResponse\",\n  \"description\": \"GetEffectivePoliciesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"effectivePolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EffectivePolicies\"\n        },\n        {\n          \"description\": \"The effective policies.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-effective-policies-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: GetEffectivePoliciesResponse
---
