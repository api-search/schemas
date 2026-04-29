---
description: Represents the request to forget the device.
layout: schema
name: ForgetDeviceRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
- description: ''
  name: DeviceKey
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-forget-device-request-schema.json
slug: user-pools-forget-device-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-forget-device-request-schema.json\",\n  \"title\": \"ForgetDeviceRequest\",\n  \"description\": \"Represents the request to forget the device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose registered device you want to forget.\"\n        }\n      ]\n    },\n    \"DeviceKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceKeyType\"\n        },\n        {\n          \"description\": \"The device key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DeviceKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-forget-device-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ForgetDeviceRequest
---
