---
description: ListTargetsForPolicyResponse schema
layout: schema
name: ListTargetsForPolicyResponse
properties_list:
- description: ''
  name: targets
  type: object
- description: ''
  name: nextMarker
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-targets-for-policy-response-schema.json
slug: iot-device-management-list-targets-for-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-targets-for-policy-response-schema.json\",\n  \"title\": \"ListTargetsForPolicyResponse\",\n  \"description\": \"ListTargetsForPolicyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyTargets\"\n        },\n        {\n          \"description\": \"The policy targets.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"A marker used to get the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-targets-for-policy-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListTargetsForPolicyResponse
---
