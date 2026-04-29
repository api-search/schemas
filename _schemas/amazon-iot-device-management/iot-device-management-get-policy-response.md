---
description: The output from the GetPolicy operation.
layout: schema
name: GetPolicyResponse
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
  name: defaultVersionId
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastModifiedDate
  type: object
- description: ''
  name: generationId
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-get-policy-response-schema.json
slug: iot-device-management-get-policy-response
source_filename: iot-device-management-get-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-policy-response-schema.json\",\n  \"title\": \"GetPolicyResponse\",\n  \"description\": \"The output from the GetPolicy operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyName\"\n        },\n        {\n          \"description\": \"The policy name.\"\n        }\n      ]\n    },\n    \"policyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyArn\"\n        },\n        {\n          \"description\": \"The policy ARN.\"\n        }\n      ]\n    },\n    \"policyDocument\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \"The\
  \ JSON document that describes the policy.\"\n        }\n      ]\n    },\n    \"defaultVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyVersionId\"\n        },\n        {\n          \"description\": \"The default policy version ID.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date the policy was created.\"\n        }\n      ]\n    },\n    \"lastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date the policy was last modified.\"\n        }\n      ]\n    },\n    \"generationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenerationId\"\n        },\n        {\n          \"description\": \"The generation ID of the policy.\"\n        }\n      ]\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-policy-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: GetPolicyResponse
---
