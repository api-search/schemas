---
description: Represents the request to get the device, as an administrator.
layout: schema
name: AdminGetDeviceRequest
properties_list:
- description: ''
  name: DeviceKey
  type: object
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Username
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-admin-get-device-request-schema.json
slug: user-pools-admin-get-device-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-get-device-request-schema.json\",\n  \"title\": \"AdminGetDeviceRequest\",\n  \"description\": \"Represents the request to get the device, as an administrator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceKeyType\"\n        },\n        {\n          \"description\": \"The device key.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\"\
  : \"The user name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DeviceKey\",\n    \"UserPoolId\",\n    \"Username\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-get-device-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AdminGetDeviceRequest
---
