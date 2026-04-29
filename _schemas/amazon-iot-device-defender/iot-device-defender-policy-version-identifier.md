---
description: Information about the version of the policy associated with the resource.
layout: schema
name: PolicyVersionIdentifier
properties_list:
- description: ''
  name: policyName
  type: object
- description: ''
  name: policyVersionId
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-policy-version-identifier-schema.json
slug: iot-device-defender-policy-version-identifier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-policy-version-identifier-schema.json\",\n  \"title\": \"PolicyVersionIdentifier\",\n  \"description\": \"Information about the version of the policy associated with the resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyName\"\n        },\n        {\n          \"description\": \"The name of the policy.\"\n        }\n      ]\n    },\n    \"policyVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyVersionId\"\n        },\n        {\n          \"description\": \"The ID of the version of the policy associated with the resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-policy-version-identifier-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: PolicyVersionIdentifier
---
