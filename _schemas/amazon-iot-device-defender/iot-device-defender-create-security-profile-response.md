---
description: CreateSecurityProfileResponse schema
layout: schema
name: CreateSecurityProfileResponse
properties_list:
- description: ''
  name: securityProfileName
  type: object
- description: ''
  name: securityProfileArn
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-create-security-profile-response-schema.json
slug: iot-device-defender-create-security-profile-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-security-profile-response-schema.json\",\n  \"title\": \"CreateSecurityProfileResponse\",\n  \"description\": \"CreateSecurityProfileResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityProfileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityProfileName\"\n        },\n        {\n          \"description\": \"The name you gave to the security profile.\"\n        }\n      ]\n    },\n    \"securityProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityProfileArn\"\n        },\n        {\n          \"description\": \"The ARN of the security profile.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-security-profile-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: CreateSecurityProfileResponse
---
