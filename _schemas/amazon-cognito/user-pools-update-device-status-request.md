---
description: Represents the request to update the device status.
layout: schema
name: UpdateDeviceStatusRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
- description: ''
  name: DeviceKey
  type: object
- description: ''
  name: DeviceRememberedStatus
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-update-device-status-request-schema.json
slug: user-pools-update-device-status-request
source_filename: user-pools-update-device-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-device-status-request-schema.json\",\n  \"title\": \"UpdateDeviceStatusRequest\",\n  \"description\": \"Represents the request to update the device status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose device status you want to update.\"\n        }\n      ]\n    },\n    \"DeviceKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceKeyType\"\n        },\n        {\n          \"description\": \"The device key.\"\n        }\n      ]\n    },\n    \"DeviceRememberedStatus\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/DeviceRememberedStatusType\"\n        },\n        {\n          \"description\": \"The status of whether a device is remembered.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessToken\",\n    \"DeviceKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-device-status-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UpdateDeviceStatusRequest
---
