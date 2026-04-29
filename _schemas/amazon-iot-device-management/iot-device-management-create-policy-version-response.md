---
description: The output of the CreatePolicyVersion operation.
layout: schema
name: CreatePolicyVersionResponse
properties_list:
- description: ''
  name: policyArn
  type: object
- description: ''
  name: policyDocument
  type: object
- description: ''
  name: policyVersionId
  type: object
- description: ''
  name: isDefaultVersion
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-policy-version-response-schema.json
slug: iot-device-management-create-policy-version-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-policy-version-response-schema.json\",\n  \"title\": \"CreatePolicyVersionResponse\",\n  \"description\": \"The output of the CreatePolicyVersion operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyArn\"\n        },\n        {\n          \"description\": \"The policy ARN.\"\n        }\n      ]\n    },\n    \"policyDocument\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \"The JSON document that describes the policy.\"\n        }\n      ]\n    },\n    \"policyVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyVersionId\"\
  \n        },\n        {\n          \"description\": \"The policy version ID.\"\n        }\n      ]\n    },\n    \"isDefaultVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IsDefaultVersion\"\n        },\n        {\n          \"description\": \"Specifies whether the policy version is the default.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-policy-version-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreatePolicyVersionResponse
---
