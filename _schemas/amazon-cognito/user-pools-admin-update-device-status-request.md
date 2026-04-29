---
description: The request to update the device status, as an administrator.
layout: schema
name: AdminUpdateDeviceStatusRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: DeviceKey
  type: object
- description: ''
  name: DeviceRememberedStatus
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-admin-update-device-status-request-schema.json
slug: user-pools-admin-update-device-status-request
source_filename: user-pools-admin-update-device-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-update-device-status-request-schema.json\",\n  \"title\": \"AdminUpdateDeviceStatusRequest\",\n  \"description\": \"The request to update the device status, as an administrator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user name.\"\n        }\n      ]\n    },\n    \"DeviceKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceKeyType\"\n        },\n        {\n       \
  \   \"description\": \"The device key.\"\n        }\n      ]\n    },\n    \"DeviceRememberedStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceRememberedStatusType\"\n        },\n        {\n          \"description\": \"The status indicating whether a device has been remembered or not.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"Username\",\n    \"DeviceKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-update-device-status-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AdminUpdateDeviceStatusRequest
---
