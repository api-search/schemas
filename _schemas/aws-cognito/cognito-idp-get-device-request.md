---
description: Represents the request to get the device.
layout: schema
name: GetDeviceRequest
properties_list:
- description: ''
  name: DeviceKey
  type: object
- description: ''
  name: AccessToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-get-device-request-schema.json
slug: cognito-idp-get-device-request
source_filename: cognito-idp-get-device-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceKeyType\"\n        },\n        {\n          \"description\": \"The device key.\"\n        }\n      ]\n    },\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose device information you want to request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DeviceKey\"\n  ],\n  \"description\": \"Represents the request to get the device.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-device-request-schema.json\",\n  \"title\": \"GetDeviceRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-device-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetDeviceRequest
---
