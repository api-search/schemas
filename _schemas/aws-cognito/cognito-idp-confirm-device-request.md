---
description: Confirms the device request.
layout: schema
name: ConfirmDeviceRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
- description: ''
  name: DeviceKey
  type: object
- description: ''
  name: DeviceSecretVerifierConfig
  type: object
- description: ''
  name: DeviceName
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-confirm-device-request-schema.json
slug: cognito-idp-confirm-device-request
source_filename: cognito-idp-confirm-device-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose device you want to confirm.\"\n        }\n      ]\n    },\n    \"DeviceKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceKeyType\"\n        },\n        {\n          \"description\": \"The device key.\"\n        }\n      ]\n    },\n    \"DeviceSecretVerifierConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceSecretVerifierConfigType\"\n        },\n        {\n          \"description\": \"The configuration of the device secret verifier.\"\n        }\n      ]\n    },\n    \"DeviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceNameType\"\n        },\n        {\n          \"description\"\
  : \"The device name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessToken\",\n    \"DeviceKey\"\n  ],\n  \"description\": \"Confirms the device request.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-confirm-device-request-schema.json\",\n  \"title\": \"ConfirmDeviceRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-confirm-device-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ConfirmDeviceRequest
---
