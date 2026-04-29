---
description: The output from the GetPolicyVersion operation.
layout: schema
name: GetPolicyVersionResponse
properties_list:
- description: ''
  name: policyArn
  type: object
- description: ''
  name: policyName
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
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastModifiedDate
  type: object
- description: ''
  name: generationId
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-get-policy-version-response-schema.json
slug: iot-core-get-policy-version-response
source_filename: iot-core-get-policy-version-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-policy-version-response-schema.json\",\n  \"title\": \"GetPolicyVersionResponse\",\n  \"description\": \"The output from the GetPolicyVersion operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyArn\"\n        },\n        {\n          \"description\": \"The policy ARN.\"\n        }\n      ]\n    },\n    \"policyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyName\"\n        },\n        {\n          \"description\": \"The policy name.\"\n        }\n      ]\n    },\n    \"policyDocument\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \"The JSON\
  \ document that describes the policy.\"\n        }\n      ]\n    },\n    \"policyVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyVersionId\"\n        },\n        {\n          \"description\": \"The policy version ID.\"\n        }\n      ]\n    },\n    \"isDefaultVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IsDefaultVersion\"\n        },\n        {\n          \"description\": \"Specifies whether the policy version is the default.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date the policy was created.\"\n        }\n      ]\n    },\n    \"lastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date the policy was last modified.\"\n        }\n\
  \      ]\n    },\n    \"generationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenerationId\"\n        },\n        {\n          \"description\": \"The generation ID of the policy version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-policy-version-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: GetPolicyVersionResponse
---
