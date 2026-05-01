---
description: GetEffectivePoliciesResponse schema
layout: schema
name: GetEffectivePoliciesResponse
properties_list:
- description: ''
  name: effectivePolicies
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-get-effective-policies-response-schema.json
slug: iot-device-management-get-effective-policies-response
source_filename: iot-device-management-get-effective-policies-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-effective-policies-response-schema.json\",\n  \"title\": \"GetEffectivePoliciesResponse\",\n  \"description\": \"GetEffectivePoliciesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"effectivePolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EffectivePolicies\"\n        },\n        {\n          \"description\": \"The effective policies.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-effective-policies-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: GetEffectivePoliciesResponse
---
