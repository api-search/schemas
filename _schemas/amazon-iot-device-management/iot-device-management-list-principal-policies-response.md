---
description: The output from the ListPrincipalPolicies operation.
layout: schema
name: ListPrincipalPoliciesResponse
properties_list:
- description: ''
  name: policies
  type: object
- description: ''
  name: nextMarker
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-principal-policies-response-schema.json
slug: iot-device-management-list-principal-policies-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-principal-policies-response-schema.json\",\n  \"title\": \"ListPrincipalPoliciesResponse\",\n  \"description\": \"The output from the ListPrincipalPolicies operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Policies\"\n        },\n        {\n          \"description\": \"The policies.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"The marker for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-principal-policies-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListPrincipalPoliciesResponse
---
