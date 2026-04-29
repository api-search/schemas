---
description: The output from the CreatePolicy operation.
layout: schema
name: CreatePolicyResponse
properties_list:
- description: ''
  name: policyName
  type: object
- description: ''
  name: policyArn
  type: object
- description: ''
  name: policyDocument
  type: object
- description: ''
  name: policyVersionId
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-policy-response-schema.json
slug: iot-device-management-create-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-policy-response-schema.json\",\n  \"title\": \"CreatePolicyResponse\",\n  \"description\": \"The output from the CreatePolicy operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyName\"\n        },\n        {\n          \"description\": \"The policy name.\"\n        }\n      ]\n    },\n    \"policyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyArn\"\n        },\n        {\n          \"description\": \"The policy ARN.\"\n        }\n      ]\n    },\n    \"policyDocument\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\"\
  : \"The JSON document that describes the policy.\"\n        }\n      ]\n    },\n    \"policyVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyVersionId\"\n        },\n        {\n          \"description\": \"The policy version ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-policy-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreatePolicyResponse
---
